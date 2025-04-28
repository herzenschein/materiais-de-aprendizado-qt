# Rota de aprendizado para iniciantes

Não há muito por aqui ainda. Contribua mandando um pull request! :)
  
Esta seção irá conter uma referência a conceitos, classes/tipos e links para as referências necessárias em uma sequência razoável para que um iniciante em Qt possa adquirir o conhecimento para criar suas próprias aplicações com alguma independência.
  
Por enquanto, fique claro: o melhor material para QtQuick/QML atualmente é o [qmlbook](https://www.qt.io/product/qt6/qml-book).
  
Segue um rascunho dos componentes numa ordem razoável. Falta polir melhor a lista, achar mais overviews e explicar detalhes importantes de cada.
    
## QtCore

### QCoreApplication

Importância: Alta

Para iniciantes: Aprender como utilizar o construtor e a função exec() é todo o necessário para continuar estudando (isso é válido para o QCoreApplication, QGuiApplication e QApplication). Adicionalmente, aprender as funções usadas para fornecer informações sobre o aplicativo.

Quando retornar: Após aprender sobre signals e slots, verificar as funções quit() e aboutToQuit().

Essencial: Sim

### qDebug, qInfo, qWarning, qCritical, qFatal

Importância: Alta, Média, Média, Média, Alta

Para iniciantes: Aprender como printar dados na tela. Adicionalmente, aprender os níveis de logging e quando usá-los.

Quando retornar:

Essencial: Sim

### QString, QChar, QByteArray

Importância: Alta, Média, Alta

Para iniciantes: Focar nas funções de manipulação de strings e de casting.

Quando retornar: Ao estudar QTextStream, assim como quaisquer classes QtWidgets que focam em texto, como QLineEdit e QTextEdit.

Essencial: Sim

### QStringView, QByteArrayView

Importância: Baixa, Baixa

Para iniciantes: Use sempre que não for modificar uma string.

Quando retornar: Quando estiver confiante em lidar com programas em C++ ou Qt e quiser adicionar uma camada a mais de segurança.

Essencial: Não

### QTime, QTimeZone, QDate, QDateTime, QCalendar

Importância: Média, Média, Média, Média, Média

Para iniciantes:

Quando retornar: Após aprender sobre timers.

Essencial: Não

### QRandomGenerator

Importância: Média

Para iniciantes: Focar nas funções generate() e bounded().

Quando retornar:

Essencial: Não

### QPoint, QLine, QRect, QSize

Importância: Média, Média, Média, Alta

Para iniciantes: O QSize é comumente utilizado como argumento em funções de outras classes do Qt.

Quando retornar: Ao começar a lidar com gráficos e multimídia.

Essencial: Não

### Object Trees and Ownership - [https://doc.qt.io/qt-6/objecttrees.html](https://doc.qt.io/qt-6/objecttrees.html)

Importância: Alta

Para iniciantes: Focar no conceito principal de gerenciamento de memória: se o objeto pai é destruído, seus objetos filhos também são destruídos.

Quando retornar: Sempre que for lidar com QObjects direta ou indiretamente.

Essencial: Sim

### Signals and Slots - [https://doc.qt.io/qt-6/signalsandslots.html](https://doc.qt.io/qt-6/signalsandslots.html)

Importância: Alta

Para iniciantes: Focar em: como criar signals e slots, sintaxe do QObject::connect, quando usar this.

Quando retornar: Ao começar a estudar QtWidgets ou QtQuick.

Essencial: Sim

### QFile, QDir, QUrl, QIODevice, QSettings, QSysInfo, QStandardPaths

Importância: Alta, Alta, Alta, Média, Alta, Baixa, Alta

Para iniciantes: Focar nas funções de abrir e fechar arquivos com QFile, no enum do QIODevice, em como lidar com arquivos ini com QSettings, em como editar arquivos de configuração do usuário via QStandardPaths (por exemplo, arquivos em XDG_CONFIG_DIR no Linux).

Quando retornar: Quando for lidar com documentos como JSON/XML, quando for lidar com QActions, assim como com diálogos do QtWidgets e QtQuick.

Essencial: Sim

### Qt Namespace - [https://doc.qt.io/qt-6/qt.html](https://doc.qt.io/qt-6/qt.html)

Importância: Alta

Para iniciantes: Foque nos enums disponíveis para o Qt e veja as classes pertinentes que os usam.

Quando retornar:

Essencial: Não

### QFlags - [https://doc.qt.io/qt-6/qflags.html](https://doc.qt.io/qt-6/qflags.html)

Importância: Baixa

Para iniciantes: Os QFlags são úteis para criar seus próprios enums de maneira segura para uso em classes ou funções.

Quando retornar:

Essencial: Não

### Container Classes - [https://doc.qt.io/qt-6/containers.html](https://doc.qt.io/qt-6/containers.html)

Importância: Alta

Para iniciantes: Se você tiver experiência com classes de container e iteradores da biblioteca padrão, não será difícil acompanhar.

Quando retornar:

Essencial: Sim

### QList, QVector

Importância: Alta, Baixa

Para iniciantes: Foque no QList do Qt6 e nas suas diferenças com os containers da biblioteca padrão. O QVector foi deprecado pelo QList. Passe um bom tempo se acostumando com o QList.

Quando retornar: Quando for estudar qualquer descendente do QList.

Essencial: Sim

### QMap, QSet

Importância: Alta, Média

Para iniciantes: Se você tiver experiência com std::map e std::set, não será difícil acompanhar. O QMap será usado extensivamente no futuro, e o QSet fornece algumas funções de conveniência para criar containers facilmente.

Quando retornar: Quando for estudar o QVariant e o QVariantMap, que pode ser usado com QJSon e QXmlStream.

Essencial: Sim

### QVariant, QIterator

Importância: Alta, Média

Para iniciantes: Se você tiver experiência com std::variant, não será difícil acompanhar. Passe bastante tempo estudando o QVariant, pois ele é necessário para a integração entre código C++ e QML no QtQuick, além de fornecer classes derivadas muito úteis como QVariantList e QVariantMap.

Quando retornar: Ao começar a estudar QtQuick.

Essencial: Sim

### QStringList, QByteArrayList

Importância: Média, Média

Para iniciantes: Se você tiver praticado lidar com o QList, não será difícil acompanhar. Foque nas diferenças de uso do QString e do QByteArray comparado às suas versões QList, assim como ao QList\<QString\> e QList\<QByteArray\>.

Quando retornar:

Essencial: Não

### QTextStream

Importância: Baixa

Para iniciantes: Esta classe é particularmente útil para implementar o equivalente a std::cout e std::cin, e age de maneira similar. Se você tiver praticado lidar com QString, QByteArray e QIODevice, não será difícil acompanhar.

Essencial: Não
  
### QVariantList, QVariantMap

Importância: Alta, Alta

Para iniciantes: Se você tiver praticado lidar com QVariant, não será difícil acompanhar. Passe bastante tempo estudando estas classes, pois elas são usadas bem comumente em programas grandes ou com estruturas de dados complexas, e são necessários para a integração entre código C++ e QML no QtQuick, além de serem úteis com QJSon e QXmlStream.

Quando retornar: Ao começar a estudar QtQuick, ou ao lidar com QJSon e QXmlStream.

Essencial: Sim

### QCommandLineParser, QCommandLineOption

Importância: Baixa, Média

Para iniciantes: Excetuando o addPositionalArgument() de QCommandLineParser, o construtor e as demais funções são simples. Foque mais no QCommandLineOption e seus construtores. É necessário ter bom entendimento do int argc (contagem de argumentos) e do char* argv[] (vetor/lista de argumentos) e seu papel ao rodar o programa em linha de comando.

Quando retornar:

Essencial: Não

### QJsonObject, QJsonDocument

Importância: Média, Média

Para iniciantes: Se você tiver praticado lidar com QFile/QIODevice/QStandardPaths, não será difícil acompanhar.

Quando retornar:

Essencial: Não

### QXmlStreamReader, QXmlStreamWriter

Importância: Média, Média

Para iniciantes: É necessário entendimento do Document Object Model (DOM), além de QFile e QByteArray, e boa prática com iteradores.

Quando retornar:

Essencial: Não

### QEvent

Importância: Alta

Para iniciantes: De início, basta focar nas opções disponíveis de seu enum. Mais tarde, ao estudar QtWidgets, convém voltar a esta classe para ver suas classes derivadas, uma vez que são necessárias para manipular eventos de interface ou dispositivos de entrada (mouse, teclado).

Quando retornar: Ao lidar com os signals e slots de QtWidgets.

Essencial: Sim

### Timers, QTimer - [https://doc.qt.io/qt-6/timers.html](https://doc.qt.io/qt-6/timers.html)

Importância: Média, Média

Para iniciantes: Excetuando callOnTimeout(), não será difícil acompanhar. Mesmo que para os seus objetivos o QTimer não seja tão útil, a classe permite facilmente testar outras classes conforme são aprendidas.

Quando retornar: Quando você começar a fazer conexões entre eventos mais complexas com QtWidgets.

Essencial: Não

---
  
## QtWidgets

* QApplication
* QWidget, QDialog
* QLabel, QLineEdit, QTextEdit, QTextBrowser
* QPushButton, QRadioButton, QCheckBox, QComboBox, QSpinBox, QSlider
* QDial, QProgressBar
* QScrollArea
* Layout Management - [https://doc.qt.io/qt-6/layout.html](https://doc.qt.io/qt-6/layout.html)
* QHBoxLayout, QVBoxLayout, QGridLayout, QFormLayout
* QAction
* QMainWindow, QMenu, QMenuBar
* QToolBar, QTabWidget
* QColor, QFont, QIcon, QImage, QStyle
* Model/View Programming - [https://doc.qt.io/qt-6/model-view-programming.html](https://doc.qt.io/qt-6/model-view-programming.html)
* Model/View Tutorial - [https://doc.qt.io/qt-6/modelview.html](https://doc.qt.io/qt-6/modelview.html)
* QListView
* QColumnView, QTableView, QTreeView
* QAbstractItemModel, QModelIndex
* QKeyEvent, QShortcut, QValidator
* Accessibility for QWidget Applications - [https://doc.qt.io/qt-6/accessible-qwidget.html](https://doc.qt.io/qt-6/accessible-qwidget.html)
* Internationalization with Qt - [https://doc.qt.io/qt-6/internationalization.html](https://doc.qt.io/qt-6/internationalization.html)


## QtQuick

* Não há nada por aqui ainda :(
