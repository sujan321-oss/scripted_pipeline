

def parmas = true 

def fruits = [ "mango" , "orange" , "apple"  ] 

node { 
       
      string name = "helli"
      
      stage("print_fruits") {
                 echo "${fruits}"
 		 echo "${fruits[0]}"  
  		} 
        
       stage("mapData") { 
        def  map_data = ["name": "khuma" , "surname": "pokharel"]
         echo "${map_data['name']}"
         
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
