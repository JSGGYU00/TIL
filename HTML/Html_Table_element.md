# HTML Table

- 테이블이란 데이터를 행과 열의 형태로 구조화하여 표시하는 방법.

- 표의 형태로 정보를 깔끔하게 정리하고 싶을 때 사용함

---

</br>

</br>

- Table의 요소 1

  - `<table>` : 테이블 전체를 감싸고 있는 태그.

  - `<th>` : 표의 첫 번째 행 테이블의 머리, 헤더 "셀"을 알려주는 태그.

  - `<td>` : 데이터를 포함한 표 안에 각각의 단일 셀을 정의함.

  - `<tr>` : 첫 번째 행 밑으로 각각의 행을 구분지어주는 태그.

</br>

- Table의 요소 2

  - `<thead>`, `<tbody>`, `<tfoot>` 태그는 테이블 구조를 구분해주는 역할을 함.

    이 요소들은 표를 섹션으로 분리하는 작업 외에는 하는 일이 없음.

  - `<thead>` : 테이블의 머리부분을 알려주는 태그. 머리의 행은 하나 이상일 수도 있음.

  - `<tbody>` : 테이블의 본문부분을 알려주는 태그. 데이블의 대부분의 데이터가 여기에 위치함.

  - `<tfoot>` : 테이블의 하단에 위치하는 부분을 알려주는 태그. 대게 합계, 요약 등 과 같은 정보를 담을 때 사용.

</br>

- Table의 요소 3

  - `rowspan` : 하나의 셀이 행을 여러 개를 차지할 때 사용한다. 표의 세로 방향으로 셀을 병합함.

    - 2개의 행을 하나로 합치고 싶다면 `rowspan="2"`를 입력.

  - `colspan` : 하나의 셀이 열을 여러 개를 차지할 때 사용한다. 표의 가로 방향으로 셀을 병합함.

    - 2개의 열을 하나로 합치고 싶다면 `colspan="2"`를 입력.

</br>

---

- 요소 3 까지의 예시

```html
<!-- example -->
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>table elements</title>
  </head>
  <body>
    <h2>V2</h2>
    <table>
      <thead>
        <tr>
          <th rowspan="2">Animal</th>
          <th colspan="2">Average mass</th>
          <th rowspan="2">Flighted</th>
        </tr>
        <tr>
          <th>kg</th>
          <th>lb</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Ostrich</td>
          <td>104</td>
          <td>230</td>
          <td>No</td>
        </tr>
        <tr>
          <td>Somali Ostrich</td>
          <td>89</td>
          <td>200</td>
          <td>No</td>
        </tr>
        <tr>
          <td>Wild turkey</td>
          <td>13.4</td>
          <td>29.3</td>
          <td>Yes</td>
        </tr>
      </tbody>
    </table>
  </body>
</html>
```
