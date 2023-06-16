---
name: "[Java]"
about: "- 자바 코딩테스트 헷갈리는 문법"
title: ''
labels: ''
assignees: ''

---

## 배열 정렬 기준을 여러개로 하는 방법 → 람다
    
👉 - 2차원 배열에서 두 가지 기준으로 정렬 

```java
    Arrays.sort(targets, (o1, o2) -> {
    	if(o1[0] != o2[0]) { // 만약 첫번째 값이 같지 않으면 첫번째 기준 오름차순
        	return o1[0]-o2[0];
    	} else { // 첫 번째 값이 같다면 두번째 기준으로 오름차순
        	return o1[1]-o2[1];
    	}
    });
```
    
👉 - 2차원 배열에서 한 가지 기준으로 정렬
    

```java
    Arrays.sort(targets,(x,y)-> x[1]-y[1]); 
    
    Arrays.sort(targets, (x,y) -> {return x[1]-y[1];});
```
   
둘 다 같은 뜻
