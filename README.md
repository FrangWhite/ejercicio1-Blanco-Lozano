<img width="778" height="524" alt="image" src="https://github.com/user-attachments/assets/cf8b9986-9f68-4ff4-8743-1c78227cee8f" />


import 'package:flutter/material.dart';
import 'package:flutter/services.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text('Blanco Lozano'),
        ),
        body: Center(
          child: Builder(
            builder: (context) {
              return Column(
                mainAxisAlignment: MainAxisAlignment.center,
                children: [
                  const Text('¡Hola Mundo!'),
                  const SizedBox(height: 20),
                  ElevatedButton(
                    onPressed: () {
                      print('¡Clic!');
                    },
                    child: const Text('Botón'),
                  ),
                ],
              );
            },
          ),
        ),
      ),
    );
  }
}
