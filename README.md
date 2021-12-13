gridsome笔记

1.templates的使用

答：templates中的模板文件访问规则设置在gridsome.config.js文件中设置，设置规则如下

templates: {
      Post: [
        {
          path: '/posts/:id',//gridsome.serve里面添加集合数据里面唯一主键这里是id
          component: './src/templates/Post.vue'
        }
      ]
	}

2.路由跳转采用的方式

答：采用的是g-link  <g-link :to="'/posts/'+post.id">{{ post.title }}</g-link>
