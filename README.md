# spin-pose-recognition

# Technical development and issues

## Main Idea

### Step 1: binary classification between spin and non-spin

- two ways:  single frame / sliding window
    
    
![90c7f7af37336b765bb78e6197815671](https://github.com/user-attachments/assets/9df9cc34-aeba-4c76-bcfb-470c74e3986c)
![1fe1645be2baa105dc39c8a822ad6f90](https://github.com/user-attachments/assets/fd934c57-9974-435f-839d-7a1684291377)

    
- Goal: automatically detect spins and their lengths
- Dataset:
    - video clips with labels of starting / ending frames of spins
    - tool: https://vidat2.davidz.cn/#/ (output format: json)
    - current progress: 0/?

### Step 2: multi-class classification between different spin postures

- approach:
    - key point (joint) recognition (demo in GitHub)
    - train model using output key point data (how ?) → classification
- Dataset:
    - single posture dataset https://drive.google.com/drive/folders/164JXKSC9NTRy1CVU9oWi94Uyltr0BsfA
        - method: trim and classify manually
        - current progress: 01-07 valid (approx. 70/100)
- Issues:
    - do we need segmentation?
    - how to count number of rotations? → do we need to develop a labelling tool

### Other issues

- Main channels of communication:
    - wechat 大群
    - GitHub issues
    - communication table made by promotion group https://docs.qq.com/sheet/DVlhJeUd5c0NDQkF0?tab=BB08J2
    - regular meetings
- licence
    - open-source or not? (dataset + model)
