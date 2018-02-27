# Qt
**Лабораторная работа #8**  
**Использование фреймворка Qt для разработки графического приложения**

**Цель работы**: 

Разработать на языке C++ с использованием кросплатформенногофреймворка с открытым исходным кодом Qt графическое приложение.

**Ход работы**:
1.  Мною был создан данный репозиторий на GitHub.
2.	А так же подключен репозиторий в среде разработки vscode
3.	Для Установки Qt на операционную систему Linux были использованы следующие команды:

#
Для обновления списка пакетов.

sudoapt-getupdate
# 
Для установки Qt.

sudo apt-get install qt5-default
#
Для установки QtCreator.

sudoapt-getinstallqtcreator
#
Для установки примеров программ на qt5(При необходимости):

sudo apt-get install qtbase5-examples qtdeclarative5-examples
#

4.	Далее я записал код создания приложения в файл main.cpp.
#
#include <QApplication>
#include <QMainWindow>
#include <QDesktopWidget>
#include <QMenuBar>

int main(intargc, char *argv[])
{
QApplicationa(argc, argv);
QMainWindow w;
QMenu *fileMenu = w.menuBar()->addMenu("&File");

QDesktopWidgetdw;
int x=dw.width()*0.7;
int y=dw.height()*0.7;
w.setFixedSize(x,y);
w.show();
returna.exec();
}
#
5.	Собрал и запустил приложение.






