# sortedunion.md
      function unite(arr1, arr2, arr3) {
      /*------------------
      var args = arguments, results = [], answer = {}, finalAnswer = [];
      
      for(var i = 0; i < args.length; i++){
         for(var j = 0; j < args[i].length; j++){
             results.push(args[i][j]);
             
         }
       
      }
      for( var t = 0; t < results.length; t++){
          answer[results[t]] = results[t];
      }
      
      for(var key in answer){
          finalAnswer.push(answer[key]);
      }
      return finalAnswer;
      ---------------*/
         var args = arguments, results = [],finalAnswer = [];
      
      for(var i = 0; i < args.length; i++){
         for(var j = 0; j < args[i].length; j++){
             results.push(args[i][j]);
             
         }
          
      }
      
       for( var t = 0; t < results.length; t++){
          if(finalAnswer.indexOf(results[t]) === -1){
              finalAnswer.push(results[t]);
          }
      }
      return finalAnswer;
       
        
      }
      
      unite([1, 3, 2], [5, 2, 1, 4], [2, 1]);
