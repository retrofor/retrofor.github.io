---
title: test
authors: [Hsiang_Nianian]
type: post
date: 2023-01-23T10:29:34.197Z
lastmod: ""
featured: /img/post/logo.png
featuredpath: img/post
draft: false
showtoc: true
---
## Test

:::tip 

bug test

```js
function Clock(props) {
  const [date, setDate] = useState(new Date());
  useEffect(() => {
    const timerID = setInterval(() => tick(), 1000);

    return function cleanup() {
      clearInterval(timerID);
    };
  });

  function tick() {
    setDate(new Date());
  }

  return (
    <div>
      <h2>It is {date.toLocaleTimeString()}.</h2>
    </div>
  );
}
```
