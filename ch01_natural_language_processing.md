# 자연어 처리(natural language processing)

자연어란 우리가 일상 생활에서 사용하는 언어를 말한다.

## 준비하기

### 아나콘다(Anaconda) 설치

머신 러닝을 위한 기본적인 파이썬 패키지들을 모아놓은 배포판.

 * 다운로드 페이지: https://www.anaconda.com/download
   - Anaconda3-2024.10-1-Windows-x86_64.exe

설치가 완료하면 Anaconda Navigator 를 실행하여 아나콘다 프롬프트 `Anaconda Prompt` 를 기동, 아래 커멘드를 입력하여 아나콘다 파이썬 패키지를 전부 최신 버전으로 업데이트 한다.

```cmd
> conda update -n base conda
> conda update --all
```

#### 참고

파이썬과 Tensorflow 의 상호 호환 맵:
https://www.tensorflow.org/install/pip?hl=ko


### 구글의 코랩(Colab)

아나콘다의 설치가 어려운 경우, Colab를 이용하여 인터넷 상에서 파이썬 실습이 가능하다. (회원가입 로그인 필요)

 * Colab: https://colab.research.google.com/


#### 파이썬 실습하기

>상단메뉴의 파일 > 새 노트북

코드를 작성하는 부분에 `3 + 5` 를 입력 후 `Shift + Enter` 를 누르면 `8` 이라는 결과값을 확인 할 수 있다.

#### 무료로 GPU 사용하기

Colab 실습 시의 장점은 GPU를 무료로 사용할 수 있다는 점이다.

>상단메뉴의 런타임 > 런타임 유형 변경 > GPU를 선택 후 저장 ( 현재 'T4 GPU' )

이 후 실습을 진행한다.

#### 파일 업로드

Colab에 데이터를 업로드 하여 해당 데이터로 실습을 할 수 있다.

> 좌측메뉴의 파일 > 세션 저장소에 업로드

업로드 후에는 파일 목록에 업로드 된 파일이 표시된다.

### 텐서플로우(Tensorflow) 설치

텐서플로우는 구글이 2015년에 공개한 머신 러닝 오픈소스 라이브러리 이다.

아나콘다 프롬프트 또는 명령 프롬프트를 통해서 설치가 가능하다.

```cmd
# 설치 커멘드
> pip install tensorflow

# 정상설치 되었는지 버전 확인
> ipython
In [1]: import tensorflow as tf
In [2]: tf.__version__
Out[2]: '2.19.0'
In [3]: exit
```

### 케라스(Keras) 설치

케라스는 딥 러닝 프레임쿼크인 텐서플로우에 대한 추상화 된 API를 제공한다.

```cmd
# 설치 커멘드
> pip install keras

# 정상설치 되었는지 버전 확인
> ipython
In [1]: import keras
In [2]: keras.__version__
Out[2]: '3.9.0'
In [3]: exit
```

### 젠심(Gensim) 설치

젠심은 머신 러닝을 사용하여 토픽 모델링과 자연어 처리 등을 수행할 수 있게 해주는 오픈 소스 라이브러리 이다.

```cmd
# 설치 커멘드
> pip install gensim

# 정상설치 되었는지 버전 확인
> ipython
...
In [1]: import gensim
In [2]: gensim.__version__
Out[2]:  '4.3.2'
In [3]: exit
```

※ 하지만, 젠심은 커멘드 입력 결과 에러가 나서 정상적으로 설치가 되지 않은 듯.

### 사이킷런(Scikit-learn) 설치

사이킷런은 파이썬 머신 러닝 라이브러리 이다.

```cmd
# 설치 커멘드
> pip install scikit-learn
# 정상설치 되었는지 버전 확인
> ipython
In [1]: import sklearn
In [2]: sklearn.__version__
Out[2]: '1.6.1'
In [3]: exit
```

### 주피터 노트북(Jupyter Notebook) 설치

주피터 노트북은 웹에서 코드를 작성하고 실행할 수 있는 오픈소스 웹 어플리케이션 이다.

```cmd
# 설치 커멘드
> pip install jupyter
# 주피터 노트북 실행 커멘드
> jupyter notebook
```

위의 `jupyter notebook` 커멘드를 치면 주피터 노트북이 실행 된다(웹 브라우저가 자동으로 열림).<br>
만약, 웹 브라우저가 실행되지 않는다면 직접 `localhost:8888` 에 접속도 가능하다.

> 메뉴상단의 파일 > 새 노트북

코드를 입력 후 `Run this cell` 을 실행하면 결과값을 확인할 수 있다.

```cmd
In [ ]: 3 + 8
Out[ ]: 11
```
