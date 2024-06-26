# Developing a Single Page App with Flask and Vue.js

### Want to learn how to build this?

Check out the [tutorial](https://testdriven.io/developing-a-single-page-app-with-flask-and-vuejs).

## Want to use this project?

1. Fork/Clone

1. Run the server-side Flask app in one terminal window:

    `--host="0.0.0.0"` to make the server accessible from open network
    ```sh
    $ cd server
    $ python3 -m venv env
    $ source env/bin/activate
    (env)$ pip install -r requirements.txt
    (env)$ flask run --port=5001 --debug --host="0.0.0.0"
    ```

    Navigate to [http://localhost:5001](http://localhost:5001)

1. Run the client-side Vue app in a different terminal window:

    `-- --host` to make the server accessible from open network
    use nvm to install nodejs first
    ```sh
    $ cd client
    $ npm install
    $ npm run dev -- --host
    ```

    Navigate to [http://localhost:5173](http://localhost:5173)


## CORS
```vue
axios.get(path,{headers: {"Access-Control-Allow-Origin": "*"}})
        .then((res) => {
          this.books = res.data.books;
        })
```
-- FROM <https://blog.csdn.net/m0_56699208/article/details/125597260>


[前后端分离-跨域问题详解](https://www.cnblogs.com/kangssssh/p/17165664.html)

[使用vite+vue+flask实现一个简单的前后端交互效果](https://blog.csdn.net/Alex_Zhugy/article/details/137230990)

[常见的六种跨域解决方案](https://www.cnblogs.com/mylqm/p/17653660.html)