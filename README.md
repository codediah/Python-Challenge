# Python-Challenge
                                            
votes = [0] * len(uniqueCand)                  votes = [0] * len(uniqueCand)
      for i in range(len(candidates)):              for i in range(len(candidates)):                                       
          if candidates[i] == uniqueCand:               if candidates[i] in uniqueCand:
             votes[i] += 1                                index = uniqueCand.index(candidates[i])
                                                          votes[index] += 1   
                                    
            
This is an example of a loop I came up with, which didn't throw errors but also didn't do what I hoped it would. I asked ChatGPT what I did wrong
and it helped clean it up so it worked the way I intended. I was setting the iteration of candidates to be equal to the entire uniqueCand list, and needed to match the values in uniqueCand to candidates to count how many votes each candidate got. Ironically I used the .index() function in the PyBank section for a very similar thing and just forgot it here.
