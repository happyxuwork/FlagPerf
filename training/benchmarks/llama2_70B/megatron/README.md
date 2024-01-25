## 模型信息
- Introduction

Llama 2, a collection of pretrained and fine-tuned large language models (LLMs) ranging in scale from 7 billion to 70 billion parameters. Meta's fine-tuned LLMs, called Llama 2-Chat, are optimized for dialogue use cases. Llama2 outperform open-source chat models on most benchmarks meta's researchers tested, and based on their human evaluations for helpfulness and safety, may be a suitable substitute for closedsource models. Meta provide a detailed description of their approach to fine-tuning and safety improvements of Llama 2-Chat in order to enable the community to build on their work and contribute to the responsible development of LLMs.

- Paper
[LLAMA2](https://arxiv.org/pdf/2307.09288.pdf) 

- 模型代码来源 

This case includes code from the LLAMA 2 COMMUNITY LICENSE AGREEMENT License open source project at:https://github.com/facebookresearch/llama-recipes/tree/main


## 数据准备

### 模型配置及tokenizer准备

本测试样例为预训练case，需要下载tokenizer，下载链接为 https://bd.bcebos.com/v1/klx-pytorch-work-bd/training/wurui04/llama2/tokenizer.model

在data_dir下创建tokenizer目录，将上述链接中的tokenizer.model文件下载到此目录中


### 数据集准备

本测试样例数据使用FlagScale-llama2预处理好的数据集，下载链接为

https://bd.bcebos.com/v1/klx-pytorch-work-bd/training/wurui04/llama_00_text_document.bin

https://bd.bcebos.com/v1/klx-pytorch-work-bd/training/wurui04/llama_00_text_document.idx

将上述两个文件放置于data_dir下。

LLAMA 2 COMMUNITY LICENSE AGREEMENT	
Llama 2 Version Release Date: July 18, 2023

"Agreement" means the terms and conditions for use, reproduction, distribution and 
modification of the Llama Materials set forth herein.

"Documentation" means the specifications, manuals and documentation 
accompanying Llama 2 distributed by Meta at ai.meta.com/resources/models-and-
libraries/llama-downloads/.

"Licensee" or "you" means you, or your employer or any other person or entity (if 
you are entering into this Agreement on such person or entity's behalf), of the age 
required under applicable laws, rules or regulations to provide legal consent and that 
has legal authority to bind your employer or such other person or entity if you are 
entering in this Agreement on their behalf.

"Llama 2" means the foundational large language models and software and 
algorithms, including machine-learning model code, trained model weights, 
inference-enabling code, training-enabling code, fine-tuning enabling code and other 
elements of the foregoing distributed by Meta at ai.meta.com/resources/models-and-
libraries/llama-downloads/.

"Llama Materials" means, collectively, Meta's proprietary Llama 2 and 
Documentation (and any portion thereof) made available under this Agreement.

"Meta" or "we" means Meta Platforms Ireland Limited (if you are located in or, if you 
are an entity, your principal place of business is in the EEA or Switzerland) and Meta 
Platforms, Inc. (if you are located outside of the EEA or Switzerland). 

By clicking "I Accept" below or by using or distributing any portion or element of the 
Llama Materials, you agree to be bound by this Agreement.

1. License Rights and Redistribution. 

      a. Grant of Rights. You are granted a non-exclusive, worldwide, non-
transferable and royalty-free limited license under Meta's intellectual property or 
other rights owned by Meta embodied in the Llama Materials to use, reproduce, 
distribute, copy, create derivative works of, and make modifications to the Llama 
Materials.  
      
      b. Redistribution and Use.  

            i. If you distribute or make the Llama Materials, or any derivative works 
thereof, available to a third party, you shall provide a copy of this Agreement to such 
third party. 
            ii.  If you receive Llama Materials, or any derivative works thereof, from 
a Licensee as part of an integrated end user product, then Section 2 of this 
Agreement will not apply to you. 

            iii. You must retain in all copies of the Llama Materials that you 
distribute the following attribution notice within a "Notice" text file distributed as a 
part of such copies: "Llama 2 is licensed under the LLAMA 2 Community License, 
Copyright (c) Meta Platforms, Inc. All Rights Reserved."

            iv. Your use of the Llama Materials must comply with applicable laws 
and regulations (including trade compliance laws and regulations) and adhere to the 
Acceptable Use Policy for the Llama Materials (available at 
https://ai.meta.com/llama/use-policy), which is hereby incorporated by reference into 
this Agreement.

            v. You will not use the Llama Materials or any output or results of the 
Llama Materials to improve any other large language model (excluding Llama 2 or 
derivative works thereof).  

2. Additional Commercial Terms. If, on the Llama 2 version release date, the 
monthly active users of the products or services made available by or for Licensee, 
or Licensee's affiliates, is greater than 700 million monthly active users in the 
preceding calendar month, you must request a license from Meta, which Meta may 
grant to you in its sole discretion, and you are not authorized to exercise any of the 
rights under this Agreement unless or until Meta otherwise expressly grants you 
such rights.
            
3. Disclaimer of Warranty. UNLESS REQUIRED BY APPLICABLE LAW, THE 
LLAMA MATERIALS AND ANY OUTPUT AND RESULTS THEREFROM ARE 
PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, 
EITHER EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, ANY 
WARRANTIES OF TITLE, NON-INFRINGEMENT, MERCHANTABILITY, OR 
FITNESS FOR A PARTICULAR PURPOSE. YOU ARE SOLELY RESPONSIBLE 
FOR DETERMINING THE APPROPRIATENESS OF USING OR REDISTRIBUTING 
THE LLAMA MATERIALS AND ASSUME ANY RISKS ASSOCIATED WITH YOUR 
USE OF THE LLAMA MATERIALS AND ANY OUTPUT AND RESULTS.

4. Limitation of Liability. IN NO EVENT WILL META OR ITS AFFILIATES BE 
LIABLE UNDER ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, TORT, 
NEGLIGENCE, PRODUCTS LIABILITY, OR OTHERWISE, ARISING OUT OF THIS 
AGREEMENT, FOR ANY LOST PROFITS OR ANY INDIRECT, SPECIAL, 
CONSEQUENTIAL, INCIDENTAL, EXEMPLARY OR PUNITIVE DAMAGES, EVEN 
IF META OR ITS AFFILIATES HAVE BEEN ADVISED OF THE POSSIBILITY OF 
ANY OF THE FOREGOING.
 
5. Intellectual Property.

      a. No trademark licenses are granted under this Agreement, and in 
connection with the Llama Materials, neither Meta nor Licensee may use any name 
or mark owned by or associated with the other or any of its affiliates, except as 
required for reasonable and customary use in describing and redistributing the 
Llama Materials.

      b. Subject to Meta's ownership of Llama Materials and derivatives made by or 
for Meta, with respect to any derivative works and modifications of the Llama 
Materials that are made by you, as between you and Meta, you are and will be the 
owner of such derivative works and modifications.

      c. If you institute litigation or other proceedings against Meta or any entity 
(including a cross-claim or counterclaim in a lawsuit) alleging that the Llama 
Materials or Llama 2 outputs or results, or any portion of any of the foregoing, 
constitutes an infringement of intellectual property or other rights owned or licensable 
by you, then any licenses granted to you under this Agreement shall terminate as of 
the date such litigation or claim is filed or instituted. You will indemnify and hold 
harmless Meta from and against any claim by any third party arising out of or related 
to your use or distribution of the Llama Materials.

6. Term and Termination. The term of this Agreement will commence upon your 
acceptance of this Agreement or access to the Llama Materials and will continue in 
full force and effect until terminated in accordance with the terms and conditions 
herein. Meta may terminate this Agreement if you are in breach of any term or 
condition of this Agreement. Upon termination of this Agreement, you shall delete 
and cease use of the Llama Materials. Sections 3, 4 and 7 shall survive the 
termination of this Agreement. 

7. Governing Law and Jurisdiction. This Agreement will be governed and 
construed under the laws of the State of California without regard to choice of law 
principles, and the UN Convention on Contracts for the International Sale of Goods 
does not apply to this Agreement. The courts of California shall have exclusive 
jurisdiction of any dispute arising out of this Agreement. 


### 数据集引用

```
@article{pile,
  title={The {P}ile: An 800GB Dataset of Diverse Text for Language Modeling},
  author={Gao, Leo and Biderman, Stella and Black, Sid and Golding, Laurence and Hoppe, Travis and Foster, Charles and Phang, Jason and He, Horace and Thite, Anish and Nabeshima, Noa and Presser, Shawn and Leahy, Connor},
  journal={arXiv preprint arXiv:2101.00027},
  year={2020}
}
```

### 框架与芯片支持情况
|            | Pytorch |
| ---------- | ------- |
| Nvidia GPU | ✅       |
| 昆仑芯 XPU | N/A     |
| 天数智芯   | N/A     |