Abstract

'We introduce associative embedding, a novel method for
supervising convolutional neural networks for the task of
detection and grouping. A number of computer vision problems
can be framed in this manner including multi-person
pose estimation, instance segmentation, and multi-object
tracking. Usually the grouping of detections is achieved with
multi-stage pipelines, instead we propose an approach that
teaches a network to simultaneously output detections and
group assignments...'


![associative embedding](https://github.com/fandulu/paper-notes/blob/master/images/Associative%20Embedding.png)

How the loss works:
Sum up all heatmaps of the same person, get the mean. 
The first loss is to compare the heatmap of the same person, it gets loss when the joint is mis-estimated.
The second loss is to compare the heatmap of different people, it get loss when different people share the same joint.
In such manner, we do not need to specify the tag id.

