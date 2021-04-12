# Practice_Web

1. **목적**
    - 학습한 언어(HTML, CSS)를 활용하여 반응형 웹 페이지 제작해보기

2. **제작기간**
    - 2021년 03월 24일 ~ 03월 27일

3. **사용언어**
    - HTML, CSS

4. **활용점**
    - 가로 길이(320px, 1024px) 맞춤 반응형 제작

    ```css
    /* >= 1024px (Desktop) */
    @media screen and (min-width: 1024px) {

    }
    ```

      가로길이 320px을 기준으로 모바일 전용 페이지를 제작하였고, 이후 '@media'를 활용하여 가로길이 1024px 이상인 상황에서 다른 형태로 나타나게 추가 제작

    - 부트스트랩 활용

    ```html
    <head>
      <!-- (생략) -->
      <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous">
    </head>
    ```

    - 'hover' 활용

    ```css
    .fill-button {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      width: 194px;
      height: 61px;
      font-weight: 700;
      font-size: 14px;
      line-height: 148%;
      border-radius: 60px;
      color: #57B3FE;
      background-color: #FFFFFF;
      margin-bottom: 16px;
      transition: background-color 300ms ease-in-out, color 300ms ease-in-out;
    }

    .fill-button:hover {
      background-color: #1100ff;
      color: #fff;
    }
    ```

      마우스 커서를 가져가면 'background-color'와 'color'가 ':hover', 'transition'에 설정해놓은 상태로 변화

    - 'netlify' 배포