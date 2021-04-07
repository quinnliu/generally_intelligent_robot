# generally intelligent robot

## Why

The goal is to build a robot with common sense & the ability to generalize to any 3 dimensional goal with a time estimate.

## How 

The following are generated images using Python 3 & various libraries like `matplotlib`, `networkx`, ...
The VCC robotic arm is coded using https://robosuite.ai

## Visualizations of general intelligence models

### Visualizations of HTM & HTW [1]
#### HTM node x=1,y=2 level=1 time_step=12.png markov graph
![t=12](https://user-images.githubusercontent.com/2585159/110558995-098f3100-8109-11eb-860a-064a5c4e1b20.png)

#### HTM node x=1,y=2 level=1 time_step=50.png markov graph
![t=50](https://user-images.githubusercontent.com/2585159/110558970-009e5f80-8109-11eb-926f-e5eddc877877.png)

#### HTM node x=1,y=2 level=1 time_step=50.png temporal groups dendrogram 
![t=50](https://user-images.githubusercontent.com/2585159/110824737-f12e2c00-8258-11eb-937e-b0343d72f89a.png)

### Visualizations of GVM [2] [3]
#### 16 edge filters visualization
![filter_scale=4 0_num_oriented_edge_features=16_display= 0c1,0c13,0c13 =](https://user-images.githubusercontent.com/2585159/111102526-49478580-851a-11eb-8418-3280a7dc9f89.png)

![filter_scale=4 0_num_oriented_edge_features=16_display= 0c2,0c13,0c13 =](https://user-images.githubusercontent.com/2585159/111102534-51072a00-851a-11eb-989c-237519c479a3.png)

![filter_scale=4 0_num_oriented_edge_features=16_display= 0c3,0c13,0c13 =](https://user-images.githubusercontent.com/2585159/111102541-55cbde00-851a-11eb-92fa-ccaf942c4cd9.png)

#### ...

![filter_scale=4 0_num_oriented_edge_features=16_display= 0c15,0c13,0c13 =](https://user-images.githubusercontent.com/2585159/111102561-63816380-851a-11eb-8fb3-80735c3814d1.png)

#### gaussian filter
![gaussian_filter_scale=4 0_num_oriented_edge_features=16_weights=False_gaussian_size=13 0](https://user-images.githubusercontent.com/2585159/111545680-6e1f4100-8744-11eb-8206-1625fe2e43be.png)

#### gabor filter radian angle = 0
![radian_angle=0 00_gabor_filter_scale=4 0_num_oriented_edge_features=16_weights=False_gabor_size=21](https://user-images.githubusercontent.com/2585159/111545698-75464f00-8744-11eb-8276-5e9093dd2689.png)

![radian_angle=0 00_gabor_filter_scale=4 0_num_oriented_edge_features=16_weights=True_gabor_size=21](https://user-images.githubusercontent.com/2585159/111545717-7d9e8a00-8744-11eb-91ba-41b84b950d9d.png)

#### gabor filter radian angle = 0.39, incrementing 16 times to 5.89
![radian_angle=0 39_gabor_filter_scale=4 0_num_oriented_edge_features=16_weights=False_gabor_size=21](https://user-images.githubusercontent.com/2585159/111545746-855e2e80-8744-11eb-84c2-f7b805c1b836.png)

![radian_angle=0 39_gabor_filter_scale=4 0_num_oriented_edge_features=16_weights=True_gabor_size=21](https://user-images.githubusercontent.com/2585159/111545756-88591f00-8744-11eb-9a1b-2545d13bc04e.png)

#### For handwritten digit "0"
#### cross_orient_max
![label=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111557141-1986c080-875a-11eb-9a11-4c9b6ca20ca3.png)

#### 16 competitor_maxs
![label=0_competitor_maxs_i=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111553300-125bb480-8752-11eb-99ed-75accfb14e34.png)

#### 16 gabor_filtered
![label=0_gabor_filtered_i=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111553319-20113a00-8752-11eb-8a4d-53e090f938c8.png)

#### 16 localized[i] = competitor_maxs <= gabor_filter_at_i
![label=0_localized 0 _num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111551847-23ef8d00-874f-11eb-8ba9-763e0f42fcdd.png)

#### localized[cross_orient_max > gabor_filtered] = 0
![label=0_i=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111553604-bb0a1400-8752-11eb-9bb2-a48d1c48a4ea.png)

#### updated background threshold = 0.001
![label=0_i=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111561808-117f4e80-8763-11eb-85db-d72fb33ff256.png)

![label=0_i=1_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111561820-15ab6c00-8763-11eb-94a3-13841c993a29.png)

#### 14 more images representing bottom up messages for handwritten digit "0"
![label=0](https://user-images.githubusercontent.com/2585159/111567375-d84bdc00-876c-11eb-8821-164d698b398c.png)

#### label=0_num_landmark_features=88_num_close_pairs=395_perturb_factor=2 0_max_lateral_connection_pixel_length=15_tolerance=4.png
![label=0_num_landmark_features=88_num_close_pairs=395_perturb_factor=2 0_max_lateral_connection_pixel_length=15_tolerance=4](https://user-images.githubusercontent.com/2585159/111684399-ab430c00-87f4-11eb-998a-bdf5ec2c19d3.png)

#### how to find 
optimal perturb factor?
optimal max_lateral_connection_pixel_length?
optimal tolerance?

#### cross channel pooling visualization

#### channel_offset = 1 factor = 1
![label=0_i=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111821772-0afeed00-88b1-11eb-8cd5-7a7111c0c2a9.png)

#### channel_offset = 2 factor = 2
![label=0_i=0_num_oriented_edge_features=16](https://user-images.githubusercontent.com/2585159/111821811-1520eb80-88b1-11eb-9cb2-33f0c5d55a60.png)

### Visualizations of VCC 2D 
#### Virtual environment with robotic arm & multiple camera point of view data to implement visual cognitive computer (VCC) architecture

![Screen Shot 2021-03-09 at 10 37 20 AM](https://user-images.githubusercontent.com/2585159/110505148-7da6e600-80c3-11eb-822c-6ea18befdc6f.png)

### Visualizations of VCC 3D with recursive calls 

### Visualizations of VCC 3D with recursive calls + grounded language understanding

## Sources
1. [how_the_brain_might_work.pdf](https://github.com/quinnliu/machineLearning/files/6109977/how_the_brain_might_work.pdf)
2. [GSM_summary.pdf](https://github.com/quinnliu/machineLearning/files/6135249/GSM_summary.pdf)
3. [GVM_details.pdf](https://github.com/quinnliu/machineLearning/files/6184058/GVM_details.pdf)
