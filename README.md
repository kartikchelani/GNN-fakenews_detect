# GNN-fakenews_detect (group 25)
## this project helps detect fake news using a GNN
### this project has taken inspitration from the paper https://arxiv.org/pdf/1902.06673v1.pdf 
### and github code https://github.com/safe-graph/GNN-FakeNews

For this project we only utilized the poltifact dataset.


Per request by the author of the paper please cite the paper using the following command in your python file:
@inproceedings{dou2021user,
  title={User Preference-aware Fake News Detection},
  author={Dou, Yingtong and Shu, Kai and Xia, Congying and Yu, Philip S. and Sun, Lichao},
  booktitle={Proceedings of the 44nd International ACM SIGIR Conference on Research and Development in Information Retrieval},
  year={2021}
}

Fake news poses a big threat to us and this project aims to detecting fake news and labeling them as True or False where True represents a tweet that is acurally true and False represnets a tweet that contains fake news. 

This project uses a Graphical Neural Network which is the best route to go down because it’s the most accurate for social media data because people are connected with one other


To run this code, 

start by installing all the requirements and dependencies 

put the data in the same directory as the python code

there are four models in this repo they all use the base of a GNN and run all models once a time using commands:

python -u MODEL NAME --feature profile --epochs 60 --lr 0.001 --nhid 128 --batch_size 100 --dataset NAME_OF_DATASET
Namespace(batch_size=128, dataset='politifact', epochs=60, feature='profile', lr=0.001, nhid=128, seed=777, weight_decay=0.001)
