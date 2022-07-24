## Venv
https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment

> venv (for Python 3) and virtualenv (for Python 2) allow you to manage separate package installations for different projects. They essentially allow you to create a “virtual” isolated Python installation and install packages into that virtual installation. When you switch projects, you can simply create a new virtual environment and not have to worry about breaking the packages installed in the other environments. It is always recommended to use a virtual environment while developing Python applications.

프로젝트 마다 별도의 패키지 설치를 관리해주기 위한 도구. 

설치 명령.
```zsh
python3 -m venv env
```

### Activating a virtual environment
가상 환경마다의 python과 pip의 실행파일을 path에 추가해준다. 
이 사실은 다음 명령의 결과를 통해서 확인할 수 있다. 

```bash
which python
```

위 명령은 python의 executable이 위치한 경로를 말해준다. 
즉, 이 명령의 결과가, project venv의 경로를 가리키고 있으면 된다.

## Class
https://docs.python.org/3/tutorial/classes.html#class-objects

### Class object
```python
class Test:
    name = "name"

    def find_all():
        return "found"


def test_class_object():
    assert Test.name == "name"
    assert Test.find_all() == "found"
```
