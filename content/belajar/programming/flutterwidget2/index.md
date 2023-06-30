---
title: "Widget Flutter Lanjutan"
date: 2023-06-22T16:12:30+08:00
draft: false

showtableofcontents: true
tags: ["Mobile Developer", "Flutter", "Widget", "Dart", "Dasar Flutter"]

series: ["Mobile Developer"]
series_order: 6
---

<h2>Widget Flutter</h2>

- Font Family
- List & List View
- Animated Container & Gesture Detector
- Flexibel Widget
- Stack
- Image

## Font Family

- From Google : https://fonts.google.com/

```yaml
flutter:
  uses-material-design: true
  fonts:
    - family: Open Sans
      fonts:
        - asset: fonts/OpenSans-VariableFont_wdth,wght.ttf
```

## List & List View

```dart {linenos=table,hl_lines=[2,23],linenostart=1}
class _MainAppState extends State<MainApp> {
  List<Widget> widgets = [];

  _MainAppState() {
    for (int i = 0; i < 40; i++) {
      widgets.add(
        Text(
          "Ini angka ke - $i",
          style: const TextStyle(fontSize: 30),
        ),
      );
    }
  }

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text("Berkah IT"),
        ),
        body: ListView(
          children: widgets,
        ),
      ),
    );
  }
}
```

## Animated Container && Gesture Detector

Animated Container : Sebuah widget container yang memiliki animasi.

Gesture Detector : Sebuah widget yang akan mendeteksi gerakan atau sentuhan jari
kepada layar handphone.

```dart {linenos=table,hl_lines=[2,14,"20-30"],linenostart=1}
class _MainAppState extends State<MainApp> {
  Random random = Random();
  // Random merupakan sebuah liblary bawaan dari flutter
  // untuk memberikan nilai random.

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text("Berkah IT"),
        ),
        body: Center(
          child: GestureDetector(
            onTap: () {
              setState(
                () {},
              );
            },
            child: AnimatedContainer(
              color: Color.fromARGB(
                255,
                random.nextInt(256),
                random.nextInt(256),
                random.nextInt(256),
              ),
              duration: const Duration(seconds: 1),
              width: 50.0 + random.nextInt(101),
              height: 50.0 + random.nextInt(101),
            ),
          ),
        ),
      ),
    );
  }
}
```

## Flexible Widget

```dart {linenos=table,hl_lines=[3,9,15],linenostart=1}
body: Column(
        children: [
          Flexible(
            flex: 1,
            child: Container(
              color: Colors.red,
            ),
          ),
          Flexible(
            flex: 2,
            child: Container(
              color: Colors.black,
            ),
          ),
          Flexible(
            flex: 1,
            child: Container(
              color: Colors.red,
            ),
          ),
      ],
    ),
```

## Stack
```dart {linenos=table,hl_lines=[3,5,10,17],linenostart=1}
body: Column(
  children: [
    Stack(
      children: [
        Container(
          color: Colors.red,
          width: double.infinity,
          height: 200,
          ),
        Container(
          color: Colors.black,
          width: double.infinity,
          height: 100,
          ),
      ],
    ),
    Container(
      color: Colors.yellow,
      width: double.infinity,
      height: 200,
    ),
  ],
),
```

## image

Pertama kita perlu membuat folder assets. Kemudian masukan file image kedalam folder assets tersebut.
![Folder asstes](img/assets.png)

Setelah itu. Kita perlu membuka pubspec.yaml kemudian mengetik nama folder "assets/" seperti dibawah ini :

```yaml {linenos=table,hl_lines=[1,"4-5"],linenostart=1}
flutter:
  uses-material-design: true

  assets:
    - assets/
```

Untuk memanggil image, kita gunakan widget Image dan menggunakan AssetImage. Kemudian memasukan "namafolder/namafile".

```dart {linenos=table,hl_lines=["2-4"],linenostart=1}
body: const Center(
          child: Image(
            image: AssetImage("assets/aizen.jpeg"),
          ),
        ),
```

