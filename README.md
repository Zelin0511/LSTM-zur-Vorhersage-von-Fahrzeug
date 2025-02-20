# LSTM与分层LSTM预测模型 - 汽车状态预测

## 简介 | Introduction | Einführung
该项目实现两种预测汽车状态的方法：
1. 直接使用 LSTM 神经网络进行预测
2. 根据物理规律，以一种顺序预测的分层 LSTM 神经网络进行预测

This project implements two methods for predicting vehicle states:
1. Direct prediction using an LSTM neural network
2. Layered LSTM prediction based on physical laws in a sequential manner

Dieses Projekt implementiert zwei Methoden zur Vorhersage des Fahrzeugzustands:
1. Direkte Vorhersage mit einem LSTM-Neuronalen Netzwerk
2. Schichtweise LSTM-Vorhersage, die Fahrzeugzustände basierend auf physikalischen Gesetzen sequenziell vorhersagt

---

## 直接预测方法 | Direct Prediction Method | Direkte Vorhersagemethode

### **使用步骤 | Usage Steps | Verwendungsschritte**
1. 将 **训练数据** 放入 `data` 文件夹中。
2. 运行 `DireckteVorhersage.py`，训练模型。
3. 将测试输入数据存储为 `input.csv`，放在当前目录中。
4. 运行 `DireckteVorhersage2.py` 进行预测。
5. 将实际结果存储为 `outputT.csv`，放在模型同一目录中。
6. 运行 `COMPARE.py`（注意修改要对比的 CSV 文件名称）查看预测结果。

**Steps:**
1. Place **training data** into the `data` folder.
2. Run `DireckteVorhersage.py` to train the model.
3. Store test input data as `input.csv` in the current directory.
4. Run `DireckteVorhersage2.py` to make predictions.
5. Save actual results as `outputT.csv` in the same directory as the model.
6. Run `COMPARE.py` (modify the CSV file names accordingly) to view the results.

**Schritte:**
1. Trainingsdaten in den Ordner `data` legen.
2. `DireckteVorhersage.py` ausführen, um das Modell zu trainieren.
3. Testeingabedaten als `input.csv` im aktuellen Verzeichnis speichern.
4. `DireckteVorhersage2.py` ausführen, um Vorhersagen zu treffen.
5. Tatsächliche Ergebnisse als `outputT.csv` im selben Verzeichnis wie das Modell speichern.
6. `COMPARE.py` ausführen (entsprechende CSV-Dateinamen anpassen), um die Ergebnisse anzuzeigen.

---

## 分层 LSTM 预测方法 | Layered LSTM Prediction Method | Schichtweise LSTM-Vorhersagemethode

### **使用步骤 | Usage Steps | Verwendungsschritte**
1. 将训练数据放入 `data` 文件夹（**不需要大量训练数据，请选择具有代表性的数据**）。
2. 将测试输入和输出数据放入 `Test` 目录，并放在 `data` 文件夹中。
3. 运行 `csv文件处理.py`，生成训练数据 `input.csv` 和 `output.csv`。
4. 运行 `PLSTM.py`，生成预测结果 `predictions.csv`。
5. 运行 `addTime.py`，为预测结果添加时间列。
6. 运行 `COMPARE.py` （注意修改要对比的 CSV 文件名称）查看预测结果。

---

## 运行环境 | Runtime Environment | Laufzeitumgebung
-pandas
-numpy
-sklearn
-tensorflow
-matplotlib
-keras

```bash
pip install tensorflow pandas numpy matplotlib
```

---

## 作者 | Author | Autor
**Zelin Zhao**

---

若有问题，欢迎提出 Issue，或者提交 PR 与我一起优化此项目。

If you have any questions, feel free to raise an issue or submit a PR to improve this project.

Falls Sie Fragen haben, erstellen Sie gerne ein Issue oder reichen Sie eine PR ein, um dieses Projekt zu verbessern.

