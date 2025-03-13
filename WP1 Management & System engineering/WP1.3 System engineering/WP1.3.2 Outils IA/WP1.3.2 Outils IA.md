-	On peut transformer un teaser en markdown avec le frontend : https://jpbrasile-phd20teaser.web.val.run
-	Outils utilisés au 8/3/2025 : townie( Val Town) , chatllm (abacus) ; roocode avec open router. Sci-hub pour la recherche de publications gratuitement  
-	Pour choisir le bon llm : https://livebench.ai/#/ 
-	Recherche batch sur perplexity : https://jpbrasile-polishedcoffeecoral.web.val.run/ 
-	On peut automatiser la création de teaser en fonction d’un contexte, de messages ciblées que l’on veut véhiculer et d’un template : 
    -	https://github.com/jpbrasile/images/blob/main/prompt%20for%20teaser 
    - En utilisant sonnet3.7 avec ce prompt (en mode thinking) et en copiant le code dans townie (Val town) on obtient sans erreur : https://jpbrasile-teaserfromstructuredprompt.web.val.run 
-	Automatisation d’un teaser adapté à un client donné. Solution de bout en bout :
    -	Utiliser sonnet 3.7 pour générer les requêtes : 
    ```
    give 100 queries prompts to do web search on this topics :" Danone activities can be enhanced by cold atmospheric plasma process. ". Give only the prompt, do not search from this prompt. Output format : json as  a list of string
    ``` 
    -	Utiliser Perplexity pour créer du contenu https://jpbrasile-polishedcoffeecoral.web.val.run/
    -	Utiiliser Sonnet 3.7 pour transformer le contenu au format teaser : "based on the given text file, i want a comprehensive text to show that Danone can benefit in integrating cold plasma process in this strategy. No code genération".
    -	Utiliser townie pour adapter le contenu précédent au contexte effitech et au format teaser standard  en mettant comme code template celui de : : https://jpbrasile-coldatmosphericplasmafordanone.web.val.run 



