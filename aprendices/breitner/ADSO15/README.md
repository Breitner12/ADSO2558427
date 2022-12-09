## Custompaint Stack y posicionado

# Main
~~~
import 'package:flutter/material.dart';
import 'package:flutter_application_1/background/back.dart';
import 'models/user.dart';
import 'widgets/template.dart';
import 'package:http/http.dart' as http;

void main() {
  runApp(Sena());
}

class Sena extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'usuarios',
      home: Scaffold(
          body: FutureBuilder<User>(
        future: getUser(),
        builder: (context, snapshot) {
          if (snapshot.connectionState == ConnectionState.done) {
            User user = snapshot.data as User;
            return Stack(children: [
              Background(),
              Positioned(
                top: 50.0,
                left: 60.0,
                right: 60.0,
                child: Container(
                  width: 190.0,
                  height: 150.0,
                  child: Image(
                    image: NetworkImage(user.avatar!),
                    height: 700.0,
                  ),
                ),
              ),
              Positioned(
                bottom: 40.0,
                left: 60.0,
                right: 60.0,
                child: Container(
                  width: 190.0,
                  height: 150.0,
                  child: Column(
                    children: [
                      SizedBox(height: 5.0),
                      Text(
                        user.nombre!,
                        style: TextStyle(
                            fontSize: 25.0, fontWeight: FontWeight.bold),
                      ),
                      SizedBox(height: 6.0),
                      Text(user.email!),
                      SizedBox(height: 6.0),
                      Row(
                        mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                        children: [
                          Icon(
                            Icons.mail,
                            color: Colors.red,
                            size: 24.0,
                          ),
                          Icon(
                            Icons.facebook,
                            color: Colors.blue,
                            size: 30.0,
                          ),
                          Icon(
                            Icons.ac_unit,
                            color: Colors.black,
                            size: 36.0,
                          ),
                        ],
                      ),
                    ],
                  ),
                ),
              ),
            ]);
          }
          return Center(child: CircularProgressIndicator());
        },
      )),
    );
  }

  Future<User> getUser() async {
    final url = Uri.https('reqres.in', '/api/users/3');
    final response = await http.get(url);
    return User(response.body);
  }
}
~~~

## User

~~~
import 'dart:convert' as convert;

class User {
  String? nombre;
  String? avatar;
  String? email;

  User(String json) {
    final JsonResponse = convert.jsonDecode(json);
    nombre = JsonResponse["data"]["first_name"];
    avatar = JsonResponse["data"]["avatar"];
    email = JsonResponse["data"]["email"];
  }
}
~~~

## Background

~~~
import 'package:flutter/material.dart';

class Background extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Container(
      height: double.infinity,
      width: double.infinity,
      child: CustomPaint(
        painter: _HeaderLoginPainter(),
      ),
    );
  }
}

class _HeaderLoginPainter extends CustomPainter {
  @override
  void paint(Canvas canvas, Size size) {
    final lapiz = new Paint();
    // Propiedades
    lapiz.color = Colors.blue;
    lapiz.style = PaintingStyle.fill;
    // lapiz.style = PaintingStyle.stroke;
    lapiz.strokeWidth = 10.0;

    final path = new Path();
    // dibujar con el path y lapiz

    // path.moveTo(0, size.height * 0.7);
    path.lineTo(0, size.height * 0.35);
    path.quadraticBezierTo(size.width * 0.2, size.height * 0.5,
        size.width * 0.4, size.height * 0.4);
    path.quadraticBezierTo(size.width * 0.7, size.width * 0.4, size.width * 0.9,
        size.width * 0.54);

    path.lineTo(size.width, size.height * 0.35);
    path.lineTo(size.width, 0);
    canvas.drawPath(path, lapiz);
  }

  @override
  bool shouldRepaint(covariant CustomPainter oldDelegate) {
    return true;
  }
}
~~~
