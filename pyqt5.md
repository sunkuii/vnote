# pyqt5
### 安装
``` 
 pip install pyqt5 -i https:/simple//pypi.mirrors.ustc.edu.cn/
 pip install pyqt5-tools -i https:/simple//pypi.mirrors.ustc.edu.cn/
 pip install pyqt5designer -i https:/simple//pypi.mirrors.ustc.edu.cn/
 ```
 
### pycharm配置designer
File->settings->Tools->External Tools

```
 -m PyQt5.uic.pyuic $FileName$ -o $FileNameWithoutExtension$.py
 ```
 
``` 
if __name__ == "__main__":
    import sys
    app=QtWidgets.QApplication(sys.argv)
    MainWindow=QtWidgets.QMainWindow()
    ui=Ui_MainWindow()
    ui.setupUi(MainWindow)
    MainWindow.show()
    sys.exit(app.exec_())
    