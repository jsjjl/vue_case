<template>

<!-- vue的模板里面 所有的内容要被一个根节点包含起来  -->

  <div id="app">  
    
      <h2>{{msg}}</h2>

      <br>
      这是一个根组件

    <br>

    <h3>{{obj.name}}</h3>

    <br>
    <hr>

    <br />


    <ul>
      <li v-for="a in list">
        {{a}}
      </li>
    </ul>

    <br>
    <hr>

    <br />

    <ul>
      <li v-for="item in list3">
          {{item.tiel}}
      </li>
    </ul>


     <br>
      <hr>

      <br />

      <ul>
        <li v-for="item in list2">
            {{item.cate}}

            <ol>
              <li v-for="news in item.list">
                  {{news.title}}
              </li>
            </ol>

        </li>
      </ul>

      <ul>
        <li v-for="a in list5">
          {{a.cate}}
          
          <ol >
            <li v-for="b in a.list">
              {{b.title}}
            </li>
          </ol>

        </li>
      </ul>

  </div>
</template>

<script>
    export default {     
      data () {  /*业务逻辑里面定义的数据*/
        return {
          msg: '你好vue',
          obj:{
            name:"zhangsna"
          },
          list:['1','2','4'],
          list1:[
            {'title':'11111'},
            {'title':'222'},
            {'title':'333333'},
            {'title':'44444'}
          ],

          list3:[
            {'tiel':'111'},
            {'tiel':'2'},
            {'tiel':'3'},
            {'tiel':'4'},
          ],
          list2:[
              {
                "cate":"国内新闻",
                "list":[
                   {'title':'国内新闻11111'},
                   {'title':'国内新闻2222'}
                ]
              },
              {
                "cate":"国际新闻",
                "list":[
                   {'title':'国际新闻11111'},
                   {'title':'国际新闻2222'}
                ]
              }

          ],
          list5: [
            {
              "cate":"234",
              "list":[
                {'title':"ewr"},
                {'title':"ewr"},
              ]
            },
             {
              "cate":"234234234",
              "list":[
                {'title':"ewr234234"},
                {'title':"ewr2342423"},
              ]
            }
          ],

        }
      }
    }
</script>


<style lang="scss">


</style>
