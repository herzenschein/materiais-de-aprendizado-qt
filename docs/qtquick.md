# Materiais sobre o QtQuick

Em Português:

- Playlist introduzindo programação com QtQuick da KDE Brasil (por Patrick Pereira) - [https://www.youtube.com/playlist?list=PL6oOWzm2QNuwGM1gUZkVm79jfvW9QaOpd](https://www.youtube.com/playlist?list=PL6oOWzm2QNuwGM1gUZkVm79jfvW9QaOpd)
- QtCon Brasil 2020: Prototipagem Rápida com QML (por Patrick Pereira) - [https://youtu.be/PgmrFTV9ric](https://youtu.be/PgmrFTV9ric)

Em Inglês:

- O livro de QML6 oficial da TQC baseado no qmlbook de Cadaques - [https://www.qt.io/product/qt6/qml-book](https://www.qt.io/product/qt6/qml-book)
- O livro de QML5 original por Cadaques - [https://qmlbook.github.io/](https://qmlbook.github.io/)
- Introduction to Qt/QML por KDAB - [https://www.youtube.com/playlist?list=PL6CJYn40gN6hdNC1IGQZfVI707dh9DPRc](https://www.youtube.com/playlist?list=PL6CJYn40gN6hdNC1IGQZfVI707dh9DPRc)
- QML Tips and Tricks por KDAB - [https://www.youtube.com/playlist?list=PL6CJYn40gN6jWHP5krsQrVGyYtKh3A3be](https://www.youtube.com/playlist?list=PL6CJYn40gN6jWHP5krsQrVGyYtKh3A3be)
- QML Programming Fundamentals and Beyond por ICS - [https://www.ics.com/events/qml-programming-fundamentals-and-beyond](https://www.ics.com/events/qml-programming-fundamentals-and-beyond)
- QML5 for Beginners por Bryan Cairns (pago) - [https://www.udemy.com/course/qml-for-beginners/](https://www.udemy.com/course/qml-for-beginners/)
- Qt Quick and QML for Beginners por Daniel Gakwaya (pago) - [https://www.udemy.com/course/qt_quick_qml_tutorial_for_beginners/](https://www.udemy.com/course/qt_quick_qml_tutorial_for_beginners/)
- Qt Quick and QML Intermediate por Daniel Gakwaya (pago) - [https://www.udemy.com/course/interfacing-qt-quick-qml-to-cpp-intermediate/](https://www.udemy.com/course/interfacing-qt-quick-qml-to-cpp-intermediate/)
- Qt Quick and QML Advanced por Daniel Gakwaya (pago) - [https://www.udemy.com/course/interfacing-qt-quick-qml-to-cpp-advanced/](https://www.udemy.com/course/interfacing-qt-quick-qml-to-cpp-advanced/)
  
Detalhes adicionais:

- O QtQuick vem com widgets mais crus por padrão, requer definir propriedades para integrar ao sistema.
- É a tecnologia recomendada caso for fazer aplicativos mobile.
- A partir do Qt 5.15 e do Qt 6.0 pra frente, é possível [fazer imports sem versionamento](https://doc.qt.io/qt-6/cmake-qt5-and-qt6-compatibility.html#versionless-commands).
- Caso queira verificar as versões das bibliotecas QML que você tem no seu sistema Linux, dentro das pastas /usr/lib64/qt5/qml e /usr/lib64/qt6/qml há arquivos chamados plugins.qmltypes para cada biblioteca. Neles, a versão mínima de cada módulo pode ser vista em linhas contendo a palavra "exports". 
- Lembre-se: filhos de um [Layout](https://doc.qt.io/qt-6/qml-qtquick-layouts-layout.html) devem usar [attached properties](https://doc.qt.io/qt-6/qtqml-syntax-objectattributes.html#attached-properties-and-attached-signal-handlers), não [anchors](https://doc.qt.io/qt-6/qtquick-positioning-anchors.html).
- Lembre-se: nunca use anchors e attached properties ao mesmo tempo no mesmo componente.
- Lembre-se: signals disponíveis ou criados pelo QML automaticamente geram signal handlers do tipo on + Nome (e em certos casos + Changed). Por exemplo, o signal clicked do [QtQuick.Controls Button](https://doc.qt.io/qt-6/qml-qtquick-controls2-button.html) possui o signal handler onClicked; o signal value do [QtQuick.Controls Slider](https://doc.qt.io/qt-6/qml-qtquick-controls2-slider.html) possui o signal handler onValueChanged. Signal handlers NÃO aparecem na documentação de referência do Qt.
- Há certos tipos QML especiais que não precisam de layout ou anchors, como o [Repeater](https://doc.qt.io/qt-6/qml-qtquick-repeater.html), porque internamente eles transferem a relação de pai/filho para cima. Por exemplo, no caso de um [ColumnLayout](https://doc.qt.io/qt-6/qml-qtquick-layouts-columnlayout.html) contendo um Repeater de [Buttons](https://doc.qt.io/qt-6/qml-qtquick-controls2-button.html), os Buttons se tornam filhos diretos do ColumnLayout.
- A nova API do CMake pro Qt6 [qt_add_qml_module](https://doc-snapshots.qt.io/qt6-dev/qt-add-qml-module.html) já cria resources para você, logo não é necessário (nem recomendado) usar o [qt_add_resources](https://doc.qt.io/qt-6/qt-add-resources.html) junto dele.
- Singletons feitos pelo QML usando pragma singleton requerem a propriedade `QT_QML_SINGLETON_TYPE` definida usandos `set_source_files_properties()`.
