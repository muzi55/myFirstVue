# 나의 첫번째 뷰입니다.

1. 카운터 만들기
   `vue`는 `React` 와 다르게 변동되는 값을

```jsx
data(){
    return{
        // 여기에 값을 저장합니다.
        count : 0,
    }
}
```

data 함수 안에 key:value 형식으로 저장합니다.
<br />
<br />
<br />
함수같은 경우에 `methods`라는 객체를 만들어 그곳에 함수를 저장합니다.

```jsx
methods:{
    increase(){
        this.count++;
    },
}
```

여기서 this를 써주지 않으면 에러가 나옵니다.
<br />
<br />
<br />

값을 사용할때는 `{{ count }}` 이런식으로 사용합니다.

2. 배열을 반복할시
   `v-for` 을 사용합니다.

```jsx
<div v-for="a in food" :key="a">{{ a }}</div>
  </div>
```

이런식으로 `for in` 문 처럼 사용해주면 된다.
