# Writing Week 7
## Prop Types
- PropTypes merupakan sebuah library yang dapat membantu dalam memeriksa tipe data props yang apabila tidak sesuai maka akan memunculkan pesan error

## Router
- React Router merupakan standar library untuk routing pada React. tandar routing berfungsi untuk membuat suatu website menjadi dynamic.
- Standar routing berfungsi untuk membuat suatu website menjadi dynamic.
- Install Prop Types:<br>
`  npm install prop-types`
- Contoh penggunaan prop types:
```
import PropTypes from 'prop-types';

function Header(props) {
  return (
    <>
      <h2>Name: {props.char}</h2>
      <h2>Age: {props.age}</h2>
    </>
  )
}

Header.propTypes = {
  char: PropTypes.string,
  age: PropTypes.number
}
```
## Redux/State Management Redux
- Redux digunakan untuk mengolah state management, Yaitu dengan menyimpan state di satu tempat, sehingga lebih mudah untuk di manage.
- Kegunaan Redux:
  - Menyimpan status aplikas
  - Mengelola status aplikasi 
  - Memberi tahu pihak yang berkepentingan ketika status aplikasi berubah
- Redux memungkinkan untuk mengelola status aplikasi di satu tempat dan membuat perubahan di aplikasi mudah untuk diprediksi dan dilacak
- Redux thunk adalah middleware yang memungkinkan untuk memanggil pembuat aksi yang mengembalikan fungsi sebagai ganti objek aksi
- Fungsi itu menerima metode pengiriman penyimpanan, yang kemudian digunakan untuk mengirim aksi sinkron di dalam isi fungsi setelah operasi asinkron selesai
- Untuk penggunaan redux thunk <br>
  `npm install redux-thunk@2.3.0`
- Cara kerja redux:<br>
  - Action : Adalah sebuah function yang mereturn sebuah objek.
  - Reducer : sebuah fungsi yang tugasnya untuk mengolah state yang ada di store.
  - Store : tempat untuk menampung state
- Contoh penggunaan redux
  - Setup   Store di App.js
    ```
     import { createStore } from "redux";
     import { composeWithDevTools } from "redux-devtools-extension";
     import rootReducer from "./reducers"; 
     const store = createStore(
     rootReducer,
     composeWithDevTools()
     )
     export default store;
    ```
  - Membuat reducer pada untuk todolist di src/store/reducers/todoReducer.js
    ```
       const initialState = {
       todos: [
         {
           id: 1,
           title: "title one",
           completed: false
         },
         {
           id: 1,
           title: "title one",
           completed: false
         }
       ]
     }
     const todoReducer = (state = initialState, action) => {
       const { type, payload} = action;
       switch(type){
         default:
           return {
             ...state
           }
       }
     }
     export default todoReducer;
    ```
  - Menggabungkan reducer-reducer didalam file src/store/reducers/index.js
    ```
      import { combineReducers} from "redux";
      import todoReducer from "./todoReducer";
      export default combineReducers({
      todoReducer
      })
    ```
  - Menghubungkan redux dan app reeact di file app.js
    ```
      import React from "react";
      import { Provider} from "react-redux";
      import store from "./store"
      const App= () => {
        return(
          <Provider store={store}>
            <div>
              <TodoApp/>
            </div>
          </Provider>
        )
      }
      export default App;
    ```
  - Mengambil data dari store
    ```
    import React from "react";
    import { connect } from "react-redux";
    const TodoApp= ({ todos }) => {
      return(
        <div>
          <h1>todo app</h1>
          {todos.map(todo =>
            <div key={todo.id}>
              <p>{todo.title}</p>
            </div>
          )}
        </div>
      )
    }
    const mapStateToProps = state => ({
      todos: state.todoReducer.todos
    })
    export default connect(mapStateToProps)(TodoApp);
    ```
- 
