
# Pythogorian Problem


// Problem 9  
// Special Pythagorean triplet  
    
 def ProjectEuler(): Unit = {
    
    var first = 0
    var second = 0
    var third = 0
    var product = 0
    
    for(first <- 1 to 1000)
    {
      for(second <- 1 to 1000 - first)
      {   
            third = 1000 - (first + second)
            
            val firstSqure = first * first
            val secondSqure = second * second
            val thirdSqure = third * third
            
            val equalToThird = firstSqure + secondSqure
                        
            val thousand = first + second + third
            
            if( equalToThird == thirdSqure && thousand == 1000 )
            {
              
               product = first * second * third
              
            }
      }
    }
    println(product)
  }
