# language-tree
Language tree to understand text

###Why? 
Do computers really understand our language? 

If you take the sentence: 

>Booth jumped into the box and aimed a single-shot, round-slug .44 caliber Henry Deringer at his head, firing at point-blank range

It really doesn't convey the meaning to a computer. Sure, a human can understand it, but what about computers?

This is the output by the Stanford Parser:

`(ROOT
  (S
    (NP (NNP Booth))
    (VP
      (VP (VBD jumped)
        (PP (IN into)
          (NP (DT the) (NN box))))
      (CC and)
      (VP (VBD aimed)
        (S
          (NP (DT a) (JJ single-shot) (, ,) (JJ round-slug) (CD .44) (NN caliber))
          (NP
            (NP (NNP Henry) (NNP Deringer))
            (PP (IN at)
              (NP
                (NP (PRP$ his) (NN head))
                (, ,)
                (NP
                  (NP (NN firing))
                  (PP (IN at)
                    (NP (JJ point-blank) (NN range))
                    )
                 )
               )
             )
           )
         )
      )
    )
  )
)`
