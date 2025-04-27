# machine-learning-homework-8--anomaly-detection-solved
**TO GET THIS SOLUTION VISIT:** [Machine Learning Homework 8- Anomaly Detection Solved](https://www.ankitcodinghub.com/product/machine-learning-solved-9/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;121242&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Machine Learning Homework 8- Anomaly Detection  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Machine Learning Homework 8 Anomaly Detection

ML TAs

Outline

● Task introduction

● Data

● Methodology

● Evaluation

● Baseline

● Report

Task Introduction

● Unsupervised anomaly detection

○ Training a model to determine whether the given image is similar with the training data.

Testing Training

Anomaly

Normal

Data

● Training data

○ 100000 human faces

● Testing data

○ About 10000 from the same distribution with training data (label 0)

○ About 10000 from another distribution (anomalies, label 1)

● Format

○ data/

|—– trainingset.npy

|—– testingset.npy

○ Shape: (#images, 64, 64, 3) for each .npy file

Methodology

Methodology

● Train an autoencoder with small reconstruction error.

● During inference, we can use reconstruction error as anomaly score.

○ Anomaly score can be seen as the degree of abnormality of an image.

○ An image from unseen distribution should have higher reconstruction error.

● Anomaly scores are used as our predicted values.

Evaluation – ROC AUC score

Why using ROC AUC score?

● If accuracy is applied, then a threshold is needed to determine the given image is an anomaly or not.

○ We only want a model that tells us how anomalous an image is.

○ e.g. MSE is a kind of anomaly score

● More about ROC curve

○ https://en.wikipedia.org/wiki/Receiver_operating_characteristic

Evaluation – ROC AUC score

● TPR = TP / (TP + FN) ● FPR = FP / (FP + TN)

https://towardsdatascience.com/understanding-auc-roc-cur ve-68b2303cc9c5

Baseline

● Simple

Multi-encoder autoencoder ○ Sample code

● Medium

○ Adjust model structure

● Strong

○ Multi-encoder autoencoder

● Boss

○ Add random noise and an extra classifier

○ Papers of anomaly detection

Add random noise and extra classifier

Report https://arxiv.org/pdf/1312.6114 https://youtu.be/YNUek8ioAJk https://youtu.be/8zomhgKrsmQ

1. Make a brief introduction about variational autoencoder (VAE). List one advantage comparing with vanilla autoencoder and one problem of VAE.

2. Train a fully connected autoencoder and adjust at least two different element of the latent representation. Show your model architecture, plot out the original image, the reconstructed images for each adjustment and describe the differences.

Report – Q2 (added at 4/26)

For instance, let z be the output of encoder. Then we can adjust the first dimension of z as follows: ● z[0] = 2 * z[0]

Note: you should use the same autoencoder and only adjust the latent representation (output of encoder).

Grading

● Simple Baseline (Public /Private) +0.5 pts / +0.5 pts

● Medium Baseline (Public /Private) +0.5 pts / +0.5 pts ● Strong Baseline (Public /Private) +0.5 pts / +0.5 pts

● Boss Baseline (Public /Private) +0.5 pts / +0.5 pts

● Code Submission +2 pts

● Report +4 pts

Submission Format

● “ID,score” in the first row

● Followed by 19636 lines of “image ID,anomaly score”

Code Submission

● Submit your code to NTU COOL

○ We can only see your last submission

○ Do not submit the model or dataset

○ If your codes are not reasonable, your final grade will be x 0.9

○ You should compress your code into a single file ■ &lt;student_id&gt;_hw8.zip

Link

● Kaggle: link

● Colab: link

Regulations

● You should NOT plagiarize, if you use any other resource, you should cite it in the reference.

● You should NOT modify your prediction files manually.

● Do NOT share codes or prediction files with any living creatures.

● Do NOT use any approaches to submit your results more than 5 times a day.

● Do NOT search or use additional data or pre-trained models.

● Your final grades x 0.9 if you violate of the above rules. ● Prof. Lee &amp; TAs preserve the rights to change the rules &amp; grades. (＊) Academic Ethics Guidelines for

Researchers by the Ministry of Science and Technology (MOST)

If any questions, you can ask us via …

● NTU COOL (Recommended)

● Email

○ The title should begin with “[hw8]”
