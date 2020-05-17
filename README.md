# General Guidance for Writing a Paper and Preparing for Code
Zhonghua Zheng (zhonghua.zheng@outlook.com)


<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [manuscript](#manuscript)
- [code](#code)

<!-- /code_chunk_output -->
## manuscript
1. name the repo `paper_xxx_journal`, e.g. `paper_UHWs_acp`
2. select `Add .gitignore:TeX`
3. add `*.DS_Store` and `paper_xxx_journal.pdf` to the `.gitignore` via webpage
4. create the following folders for different paper versions  
   - 0_template  
   - 1_draft
   - 2_submitted  
   - 3_response_to_reviewers  
   - 4_revised  
   - 5_final  
   - 6_proofs   
5. within each folder
   - name the latex file the same: `paper_xxx_journal.tex`
   - name the bibtex file `refs_xxx_journal.bib  `
   - make a subdir for graphics called “`graphics`”  
## code
1. name the repo `code_xxx_journal_private`, e.g. code_UHWs_acp_private
2. select `Add .gitignore:Python` (or others)
3. add `*.DS_Store` to the `.gitignore` via webpage
4. create the following folders for different paper versions  
   - misc
   - model
   - data
   - 0_scratch  
   - 1_draft
   - 2_submitted
   - 3_response_to_reviewers  
   - 4_revised  
   - 5_final  
   - 6_proofs  
5. create [symbolic link](https://apple.stackexchange.com/questions/115646/how-can-i-create-a-symbolic-link-in-terminal)
   ```bash
   ln -s ./data ./0_scratch/data
   ln -s ./data ./1_draft/data
   ln -s ./data ./2_submitted/data
   # to remove the link
   # rm -rf ./0_scratch/data
   # rm -rf ./1_draft/data
   # rm -rf ./2_submitted/data
   ```
6. Before submitting the paper, using `2_submitted` to check the code
