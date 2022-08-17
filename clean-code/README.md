# 이름
## 단순한 것과 명시적인 것은 다르다
다음 코드는 단순하다. 

```java
public List<int[]> getThem() {
	List<int[]> list1 = new ArrayList<>();

	for (int[] x : theList) {
		if (x[0] == 4) {
			list1.add(x);
		}
	}

	return list1;
}
```

하지만 위 코드는 이해하기 어렵다. 그 이유는 코드가 충분히 명시적이지 않아서 이다. 
각 부분의 `의미`가 충분히 설명되지 않았다. `의미` 란 다양하다. 배열에 무엇이 들었는지, 조건문에서 특정값이 왜 중요한지, 어떤 뜻을 갖는지, 반환값을 어떻게 사용하는지 등의 정보들을 생각할때, 의미라고 말한다. 

의미를 드러내는 방식으로 코드를 바꾸면 다음과 같다.
```java
public List<int[]> getFlaggedCells() {
	List<int[]> flaggedCells = new ArrayList<int[]>();
	
	for (int[] cell : gameBoard) {
		if (cell[STATUS_VALUE] == FLAGGED) {
			flaggedCells.add(cell);
		}
	}

	return flaggedCells;
}

```

위 코드는 명시적이다. 자연어로 설명도 가능하다.  `cell`,  `FLAGGED` 가 갖는 의미에 따라서, 외부에서 어떻게 사용해야 할지도 알 수 있다.