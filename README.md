# arrdata-map
import 'package:flutter/material.dart';
import 'package:thirdapp/Indro.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  var arrList = [
    {
      'image': 'lib/asset/a1.jpg',
      'Name': 'Suraj',
      'mobile': '7081461044',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a2.jpg',
      'Name': 'Mohan',
      'mobile': '415264855',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a3.jpg',
      'Name': 'Aakasg',
      'mobile': '708461031564',
      'unread0': '5'
    },
    {
      'image': 'lib/asset/a1.jpg',
      'Name': 'Suraj',
      'mobile': '7081461044',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a2.jpg',
      'Name': 'Mohan',
      'mobile': '415264855',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a3.jpg',
      'Name': 'Aakasg',
      'mobile': '708461031564',
      'unread0': '5'
    },
    {
      'image': 'lib/asset/a1.jpg',
      'Name': 'Suraj',
      'mobile': '7081461044',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a2.jpg',
      'Name': 'Mohan',
      'mobile': '415264855',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a3.jpg',
      'Name': 'Aakasg',
      'mobile': '708461031564',
      'unread0': '5'
    },
    {
      'image': 'lib/asset/a1.jpg',
      'Name': 'Suraj',
      'mobile': '7081461044',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a2.jpg',
      'Name': 'Mohan',
      'mobile': '415264855',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a3.jpg',
      'Name': 'Aakasg',
      'mobile': '708461031564',
      'unread0': '5'
    },
    {
      'image': 'lib/asset/a1.jpg',
      'Name': 'Suraj',
      'mobile': '7081461044',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a2.jpg',
      'Name': 'Mohan',
      'mobile': '415264855',
      'unread0': '2'
    },
    {
      'image': 'lib/asset/a3.jpg',
      'Name': 'Aakasg',
      'mobile': '708461031564',
      'unread0': '5'
    },
  ];

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
          appBar: AppBar(title: Text('Contact Number')),
          body: Container(
            child: ListView(
              children: arrList.map((value) {
                return ListTile(
                    leading: CircleAvatar(
                        child: Image.asset(
                      value['image'].toString(),
                    )),
                    title: Text(value['Name'].toString()),
                    subtitle: Text(value['mobile'].toString()),
                    trailing: CircleAvatar(
                        backgroundColor: Colors.green,
                        child: Text(value['unread0'].toString())));
              }).toList(),
            ),
          )),
    );
  }
}
