# my_second_angular_excersise
<html ng-app>
    <head>
        <title>angular</title>
        <script src="angular.js"></script>
    </head>
    <body ng-init="dayoftime=14">
        <h1>hello angular!</h1>
        <p ng-if="dayoftime < 12">good morning</p>
         <p ng-if="dayoftime > 12">good evening</p>
         <p>the day of time is : {{dayoftime}}</p>
         <span ng-bind="dayoftime"> </span> <! can be use to represent the content of veriable-->
         <br>
         <span > {{dayoftime}}</span><!same as line no10mecanism and we can write down that without curly bracket-->
         <br>
         {{dayoftime}}

         <br>
         <input type="text" ng-model="name1" placeholder="enter your name" >
         <p>your name is:{{name1}}
        <br>
          <input type="text" ng-init="age1" placeholder="enter your age" >
         <p>your age is:{{age1}}   <!this is not work because of in his case we need
                                    to get values from the txtbox; we use modelinsted 
                                    of init-->
             
         <br><input type="password">
         <input type="button">
         <br> <br> <br> <br>
         <pre>
        multipication  {{5*5}}
        diviation      {{5/5}} 
        addition       {{5+5}}
        substraction   {{5-5}}  use value 5 for all exapressions
         </pre>
        multipication  {{5*5}}<br>
        diviation      {{5/5}} <br>
        addition       {{5+5}}<br>
        substraction   {{5-5}}<br>  use value 5 for all exapressions
         </p><br>
         <p ng-init="number=10">
            veriable multiplication= {{number*number}}<br>
            two veriable addition={{dayoftime+number}}
            <br><br>
            /*array*/
            <p  ng-init="num=[1,2,3,4]"></p>
                <p>{{num[1]}}</p>
                {{num[0]+num[2]}}
            <p  ng-init="meat=['pork','chicken','bife']"></p>
            {{meat[1]}}
            {{number+num[1]}}
    </body>
</html>
