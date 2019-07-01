# webquiz

Structure du document Latex : 


     \documentclass{webquiz} 
     \title{Quiz 1: Complex numbers} 
 
     \UnitCode{MATH1001} 
     \UnitName{Differential Calculus} 
     \UnitURL{/u/UG/JM/MATH1001/} 
     \QuizzesURL{/u/UG/JM/MATH1001/Quizzes/} 
 
     \begin{document} 
 
     \begin{discussion}[short heading][optional heading] 
        . . . % optional discussion 
     \end{discussion} 
 
     \begin{question} % question 1 
        . . . 
     \end{question} 
 
     \begin{question} % question 2 
        . . . 
     \end{question} 
     . 
     . 
     \end{document}

## Créer des questions

Pour créer des questions la structure est la suivante : 

     \begin{question} 
     . . .question text 
     \begin{choice} 
      \(in)correct . . . text for (in)correct option 
      \feedback   . . . feedback on response 
 
      \(in)correct . . . text for (in)correct option 
      \feedback   . . . feedback on response 
      . 
      . 
      . 
     \end{choice} 
      \end{question}
   
Il est possible de créer 3 types de questions différentes :
 
#### Question à réponse unique

    \begin{choice} 
      \(in)correct . . . text for (in)correct option 
      \feedback   . . . feedback on response 
 
      \(in)correct . . . text for (in)correct option 
      \feedback   . . . feedback on response 
      . 
      . 
      . 
    \end{choice} 
  
  
#### Question à réponse multiple

      \begin{choice} [multiple]
      \(in)correct . . . text for (in)correct option 
      \feedback   . . . feedback on response 
 
      \(in)correct . . . text for (in)correct option 
      \feedback   . . . feedback on response 
      . 
      . 
      . 
    \end{choice} 
  
  
  #### Question à réponse avec un champs de texte
  
      \begin{question} 
         . . .question text. . . 
         \answer[*][complex|integer|lowercase|number|string]{actual answer} 
         \whenRight . . . feedback when right (optional) 
         \whenWrong . . . feedback when wrong (optional) 
       \end{question}
  
  
  
  ### Documentation simple : https://ctan.crest.fr/tex-archive/macros/latex/contrib/webquiz/doc/webquiz-online-manual.pdf
  ### Documentation complète : http://ctan.tetaneutral.net/macros/latex/contrib/webquiz/doc/webquiz.pdf
