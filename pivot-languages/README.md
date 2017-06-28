Scripts to run phrase pivot translation

    ./run-pivot-languages.sh

# data
Asian Language Treebank

# train baseline
    
    ./scripts/translation-model.sh src_lang trg_lang
    
    ./scripts/tuning-mira.sh src_lang trg_lang
    
    ./scripts/decode.sh src_lang trg_lang
    
# phrase pivot translation

changes pivot language at the pvt_lang

    ./scripts/triangulation.sh src_lang trg_lang pvt_lang
    
    for example: 
    ./scripts/triangulation.sh ms vi en
    ./scripts/triangulation.sh ms vi id
    
# multi-pivot

pivoting via more than one pivot language
      
      ./scripts/multi-pivot.sh src_lang trg_lang pvt1_lang pvt2_lang pvt3_lang
      
     for example: ./scripts/multi-pivot.sh ms vi en fil id