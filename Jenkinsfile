

def parmas = true 

def fruits = [ "mango" , "orange" , "apple"  ] 


def TestStep = [:]


properties {
	[
		parameters([
			string(name:"Username" , defaultvalue:"khuma pokharel",description:"enter your name")
		])
	]
}





node { 
       
      string name = "helli"

	  stage("dynamically_adding_teststep"){
		  echo "adding the test steps"
		  TestStep['name'] = "khuma pokharel"

		  for (int i=0;i<5;i++) { 
			  TestStep["tasks-${i}"] = "${i}"
		  }
	  }

	  stage("printing_dynamically_added_variable"){
		  echo "printing dynamically added varibale" 
		   TestStep.each{ key ,value -> println "key ${key} and value is ${value}"
		   }
	  }



      
      stage("print_fruits") {
                 echo "${fruits}"
 		 echo "${fruits[0]}"  
  		} 
        
       stage("mapData") { 
        def  map_data = ["name": "khuma" , "surname": "pokharel"]
         echo "${map_data['name']}"
         
      }    

     
      stage("makeingcomplicatedmap") { 
  			def map_data= [[
				"name" : "khuma pokharel"  
  				] 
				,
				 [
 				   "age" : 21
				] ]
                      echo " printing the name " 

                     echo "${map_data[0]['name']}"
                    
 		 }
   



        
   
     stage("clone-repo")  {
                            echo "cloning the github"   
    			    echo "printing the name of a file " 
  			    echo "$name" 

 			} 
      
	stage("productionize") { 
  
               echo "productionize the application "
  		echo "$parmas" 
            } 

        



 }   
