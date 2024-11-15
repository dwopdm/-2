https://wandb.ai/3307915720-/NLPDL-Assignment2?nw=nwuser3307915720实验结果
# -2
accuracy永远与micro_f1相等
roberta-base表现最好
agnews训练出来效果好

任务三中
![image](https://github.com/user-attachments/assets/489c9af3-c863-4598-b125-8da26a89c7c5)
我们用了两个随机种子，每个模型每个数据集运行了两次，acl数据集最差，res第二，agnews最好


$$ 4n+(34bh+5b^2a)l $$ 我们取 $$ h=3200, a=32, l=26, b=64, n=3\times 10^9 $$ 即需要约45.44GB的空间
LoRA的可训练参数大约有30M参数，我们需要存储原始模型、梯度、中间激活层等参数。同时假定LoRA的中间激活层与原始模型相同，则大约有24.27GB需要存储，节省了21.17GB
