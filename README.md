# Data-Visualization

Data Visualization is a presentation of the data in a pictorial format or graphical format.

Visualizations using 

[1.Matplotlib](https://github.com/JeyrajK/Data-Visualization/blob/master/Data%20Visualization%20-%201.ipynb) </br>
[2.Pandas - Data Visualization](https://github.com/JeyrajK/Data-Visualization/blob/master/Data%20Visualization%20-%202.ipynb) </br>
[3.Seaborn](https://github.com/JeyrajK/Data-Visualization/blob/master/Data%20Visualization%20-%203.ipynb) </br>
[4.TensorBoard](https://github.com/JeyrajK/Data-Visualization/blob/master/Data%20Visualization%20-%204.ipynb) </br>

## Matplotlib

* Excellent Data Visualization Library
* Multi-Platform Support
* It supports several plots like line, bar, scatter, histogram etc.

## Pandas - Data Visualization

Pandas uses the standard convention for referencing the matplotlib API.

## Seaborn

* Seaborn is a Python data visualization library based on matplotlib. 
* It provides a high-level interface for drawing attractive and informative statistical graphics.
* Seaborn will provide a variety of visualization patterns than matplotlib.

## TensorBoard

TensorBoard provides the visualization and tooling needed for machine learning experimentation:
    
   * Tracking and visualizing metrics such as loss and accuracy
   * Visualizing the model graph (ops and layers)
   * Viewing histograms of weights, biases, or other tensors as they change over time
   * Projecting embeddings to a lower dimensional space
   * Displaying images, text, and audio data
   * Profiling TensorFlow programs
   
### TensorBoard - Installation Steps 

    pip install tensorboard
    (upgrade the torch,tensorboard,tensorflow)
    pip install --upgrade torchvision
    pip install --upgrade torch
    pip install --upgrade tensorboard
    pip install --upgrade tensorflow  
    
**Note**
     
    supported versions 
    pytorch version - greater than 1.1.0
    torchvision version  - greater than 0.3.0
    tensorboard version - greater than 1.15

### TensorBoard - Command for Run

Run the  **tensorboard --logdir=runs** in command prompt.

Open http://localhost:6006/ to see the results.

To quit , press CRTL+C.

**Alternative Method**

    Open from Jupyter-Notebook using magic comments
    %load_ext tensorboard      
    %tensorboard --logdir logs 
   
![](https://github.com/JeyrajK/Data-Visualization/blob/master/Gifs/tensorboard-word-emb-gif.gif)
![](https://github.com/JeyrajK/Data-Visualization/blob/master/Gifs/tensorboard-img-gif.gif)
![](https://github.com/JeyrajK/Data-Visualization/blob/master/Gifs/tensorboard-dif-visu-gif.gif)

### Tensorboard dashboards

### Scalar Dashboard

<p>
    TensorBoard's Scalar Dashboard visualizes scalar statistics that vary over time; for example, you might want to track the model's loss or learning rate. you can compare multiple runs, and the data is organized by tag. The line charts have the following interactions:

    Clicking on the small blue icon in the lower-left corner of each chart will expand the chart

    Dragging a rectangular region on the chart will zoom in

    Double clicking on the chart will zoom out

    Mousing over the chart will produce crosshairs, with data values recorded in the run-selector on the left.

    Additionally, you can create new folders to organize tags by writing regular expressions in the box in the top-left of the dashboard.
</p>

### Histogram Dashboard

<p>
    The HistogramDashboard displays how the statistical distribution of a Tensor has varied over time. It visualizes data recorded via tf.summary.histogram. Each chart shows temporal "slices" of data, where each slice is a histogram of the tensor at a given step. It's organized with the oldest timestep in the back, and the most recent timestep in front. By changing the Histogram Mode from "offset" to "overlay", the perspective will rotate so that every histogram slice is rendered as a line and overlaid with one another.
</p>

### Distribution Dashboard

<p>
    The Distribution Dashboard is another way of visualizing histogram data from tf.summary.histogram. It shows some high-level statistics on a distribution. Each line on the chart represents a percentile in the distribution over the data: for example, the bottom line shows how the minimum value has changed over time, and the line in the middle shows how the median has changed. Reading from top to bottom, the lines have the following meaning: [maximum, 93%, 84%, 69%, 50%, 31%, 16%, 7%, minimum]. These percentiles can also be viewed as standard deviation boundaries on a normal distribution: [maximum, μ+1.5σ, μ+σ, μ+0.5σ, μ, μ-0.5σ, μ-σ, μ-1.5σ, minimum] so that the colored regions, read from inside to outside, have widths [σ, 2σ, 3σ] respectively.
</p>

### Image Dashboard

<p>
    The Image Dashboard can display pngs that were saved via a tf.summary.image. The dashboard is set up so that each row corresponds to a different tag, and each column corresponds to a run. Since the image dashboard supports arbitrary pngs, you can use this to embed custom visualizations (e.g. matplotlib scatterplots) into TensorBoard. This dashboard always shows you the latest image for each tag.
</p>

### Audio Dashboard

<p>
    The Audio Dashboard can embed playable audio widgets for audio saved via a tf.summary.audio. The dashboard is set up so that each row corresponds to a different tag, and each column corresponds to a run. This dashboard always embeds the latest audio for each tag.
</p>

### Graph Explorer

<p>
    The Graph Explorer can visualize a TensorBoard graph, enabling inspection of the TensorFlow model. To get best use of the graph visualizer, you should use name scopes to hierarchically group the ops in your graph - otherwise, the graph may be difficult to decipher. For more information, including examples, see the graph visualizer tutorial.
</p>

### Embedding Projector

<p>
    The Embedding Projector allows you to visualize high-dimensional data; for example, you may view your input data after it has been embedded in a high- dimensional space by your model. The embedding projector reads data from your model checkpoint file, and may be configured with additional metadata, like a vocabulary file or sprite images. 
</p>

### Text Dashboard

<p>
    The Text Dashboard displays text snippets saved via tf.summary.text. Markdown features including hyperlinks, lists, and tables are all supported.
</p>   
   
