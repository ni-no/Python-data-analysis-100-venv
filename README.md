# Python-data-analysis-100-venv
[Python実践データ分析100本ノック*](https://www.shuwasystem.co.jp/book/9784798058757.html)のためのvenvを使った仮想環境構築方法と，ライブラリ一括インストール用のファイルを公開しています．  
anacondaが重かったり，condaでサポートされていないPythonライブラリを利用したい場合にご活用ください．  
公開されているサンプルコードを用いて作動確認済みです．  
ただし，出版社さんとは関係なく，公開しているので，自己責任でご利用ください．  
また，mecabやOpenCV等の外部環境の構築には対応していません．  
cloneするより，`requirements.txt`をダウンロードすることをおすすめします．  
  
  
*下山輝昌，松田雄馬，三木孝行 著(秀和システム)  

## インストール
```
$python -m venv <ProjectName> # venvで仮想環境作成
$source <ProjectName>/bin/activate # 仮想環境のactivate
$pip install -r requirements.txt # ライブラリの一括インストール
```

`<ProjectName>`は適切なものを決めて下さい．  
`<ProjectName>`内に`requirements.txt`を配置し，インストールを行なってください．  
標準の実行環境がPython2.x系の場合は`python3`で実行してください．  

## jupyter notebookの起動
```
$source <ProjectName>/bin/activate # 仮想環境のactivate
$jupyter notebook # jupyter notebookの起動
```
ブラウザでjupyter notebookが起動されます．

終了時は`$deactive`でvenvを終了してください．

## 動作確認環境
macOS Mojave 10.14.6
Python 3.7.1
pip 18.1

## 諸注意
確認している限りでは`dlib`のインストール時にエラーが発生する場合があります．  
macの方は`$brew install cmake`で`cmake`を入れると解決する場合があります．  

## インストールされるライブラリの一覧
```
Package            Version 
------------------ --------
appnope            0.1.0   
attrs              19.3.0  
backcall           0.1.0   
bleach             3.1.0   
cycler             0.10.0  
decorator          4.4.1   
defusedxml         0.6.0   
dlib               19.18.0 
entrypoints        0.3     
importlib-metadata 1.1.0   
ipykernel          5.1.3   
ipython            7.10.1  
ipython-genutils   0.2.0   
ipywidgets         7.5.1   
jedi               0.15.1  
Jinja2             2.10.3  
joblib             0.14.0  
jsonschema         3.2.0   
jupyter            1.0.0   
jupyter-client     5.3.4   
jupyter-console    6.0.0   
jupyter-core       4.6.1   
kiwisolver         1.1.0   
MarkupSafe         1.1.1   
matplotlib         3.1.2   
mecab-python3      0.996.2 
mistune            0.8.4   
more-itertools     8.0.0   
nbconvert          5.6.1   
nbformat           4.4.0   
networkx           2.4     
notebook           6.0.2   
numpy              1.17.4  
opencv-python      4.1.2.30
ortoolpy           0.2.25  
pandas             0.25.3  
pandocfilters      1.4.2   
parso              0.5.1   
pexpect            4.7.0   
pickleshare        0.7.5   
pip                10.0.1  
prometheus-client  0.7.1   
prompt-toolkit     2.0.10  
ptyprocess         0.6.0   
PuLP               2.0     
Pygments           2.5.2   
pyparsing          2.4.5   
pyrsistent         0.15.6  
python-dateutil    2.8.1   
pytz               2019.3  
pyzmq              18.1.1  
qtconsole          4.6.0   
scikit-learn       0.22    
scipy              1.3.3   
Send2Trash         1.5.0   
setuptools         39.0.1  
six                1.13.0  
terminado          0.8.3   
testpath           0.4.4   
tornado            6.0.3   
traitlets          4.3.3   
wcwidth            0.1.7   
webencodings       0.5.1   
widgetsnbextension 3.5.1   
xlrd               1.2.0   
zipp               0.6.0 
```

Copyright 2019 ni-no
