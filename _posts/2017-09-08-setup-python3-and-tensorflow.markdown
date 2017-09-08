---
layout: post
title:  "Python3와 tensorflow 설치법"
date:   2017-09-08 12:52:41 +0900
categories: jekyll update
---
여기에 기술된 내용엔 틀린 부분 또는 부족한 부분이 있을 수 있습니다.

개인적으로 Machine Learning을 공부할 환경을 셋업하면서 관련해서 필요한 내용들을 정리해서 기술하지만, 아직 학습이 부족해서 틀린 부분 또는 부족한 부분이 있을 수 있으며, 그런 부분들이 발견되면 지속적으로 업데이트를 해나갈 생각입니다.

홍콩과기대 김성훈교수님의 강의를 보며서 예제들을 따라하다 보면 아래와 같은 에러 메세지를 볼 수가 있습니다.

{% highlight Error Message %}
(tensorflow) june@MacBookPro ~/GitHub/hunkim/DeepLearningZeroToAll$
python lab-03-1-minimizing_cost_show_graph.py
Traceback (most recent call last):
  File "lab-03-1-minimizing_cost_show_graph.py", line 3, in <module>
    import matplotlib.pyplot as plt
  File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/matplotlib/pyplot.py", line 115, in <module>
    _backend_mod, new_figure_manager, draw_if_interactive, _show = pylab_setup()
  File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/matplotlib/backends/__init__.py", line 32, in pylab_setup
    globals(),locals(),[backend_name],0)
  File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/matplotlib/backends/backend_macosx.py", line 19, in <module>
    from matplotlib.backends import _macosx
RuntimeError: Python is not installed as a framework. The Mac OS X backend will not be able to function correctly if Python is not installed as a framework. See the Python documentation for more information on installing Python as a framework on Mac OS X. Please either reinstall Python as a framework, or try one of the other backends. If you are using (Ana)Conda please install python.app and replace the use of 'python' with 'pythonw'. See 'Working with Matplotlib on OSX' in the Matplotlib FAQ for more information.
(tensorflow) june@MacBookPro ~/GitHub/hunkim/DeepLearningZeroToAll$ pythonw lab-03-1-minimizing_cost_show_graph.py
Traceback (most recent call last):
  File "lab-03-1-minimizing_cost_show_graph.py", line 2, in <module>
    import tensorflow as tf
ImportError: No module named tensorflow

{% endhighlight %}

python을 framework 으로 install 을 해야한다고 하네요.
그런데, virtualenv 환경에서 python3를 framework으로 동작하게 설정하는 방법을 정확하게 설명한 곳을 찾기는 힘들어서 그냥 다시 tensorflow 를 native app 으로 install 했습니다.
그리고, python3 는 아래와 같은 방식으로 framework 으로 설치를 했습니다.

{% highlight python3 installation %}
brew install python3 --framework
{% endhighlight %}
