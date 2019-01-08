# js-goto
js实现部分goto功能 （continue,break）语句可以都带一个标签



        
       foo:for(var i=0;i<4;i++){
             for(var j=0;j<4;j++){
                 if((i*j)>=3){
                  console.log(i.j)
                  break foo;
                 }
                 console.log(i,j)
             }
       }


        
     foo:for(var i=0;i<4;i++){
             for(var j=0;j<4;j++){
                 if(i==j){
                  //console.log(i.j)
                  continue foo;
                 }
                 //console.log(i,j)
                 if((j*i)%2===1){
                     continue
                 }

             }
       }
      



       function bar(){
           b:{
               console.log("hello")
                   break b
               console.log("ggggg")
           }
           console.log("word")
       }

    bar()  // hello word
