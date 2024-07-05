# errors
A collection of errors i faced and some solutions


## NextJs
warning: Prop `style` did not match. Server: "background-image:url(.....
<details>
  <summary>Solution</summary>

  ### 01

  ### Error
  ```js
<div>
    style={{
       backgroundImage: `url("${url}")`,
       rotate: Math.random() < 0.5 ? "15deg" : "-15deg",
    }}
</div>
  ```
  ### Solution
  ```js
<div>
    style={{
       backgroundImage: `url("${url}")`,
       rotate: [1, 2, 5].includes(key) ? "15deg" : "-15deg",
    }}
</div>
  ```
</details>
