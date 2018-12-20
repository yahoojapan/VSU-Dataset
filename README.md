# Visual Scenes with Utterances Dataset

With the widespread use of intelligent systems, more and more people expect such systems to understand complicated social scenes. 
To facilitate development of intelligent systems, we created a mock dataset called Visual Scenes with Utterances (VSU) that contains a vast body of image variations in visual scenes with an annotated utterance and a corresponding addressee. 
Our dataset is based on images and annotations from the GazeFollow dataset (Recasens et al., 2015). The GazeFollow dataset consists of (1) the original image, (2) cropped speaker image with head location annotated, and (3) gaze. 
To create our dataset, we further annotated (4) utterances in texts, and (5) to whom an utterance is addressed.
The images are available at http://gazefollow.csail.mit.edu/ .

## License

[Creative Commons Attribution 4.0 License](https://creativecommons.org/licenses/by/4.0/legalcode)

## VSU Dataset 1.0 (ARVSU -- Addressee Recognition in Visual Scenes with Utterances)

We used the first version of our dataset to develop a multi-modal deep-learning-based model to predict the conversational addressee from a specific speaker’s view.  This version is called ARVSU in the IJCAI paper as the application is addressee recognition.

### Annotation Format

The annotations are stored in a single TSV file.
The description of each field of the file is as follows:
* `id`: a unique identifier for VSU annotation
* `gfid`: an annotation ID of the GazeFollow dataset 
* `image`: an image file name in the GazeFollow dataset
* `addressee`:
  * A list of addressee types separated by commas.
  * Possible addressee types: `line_of_sight`, `photographer`, `monologue`, `others`, `not_applicable`
  * Please consult our paper for the detail of each addressee type
* `utterance`: an utterance (text) of the person in the image

### Citation

```
@inproceedings{ijcai2018-214,
  title     = {Deep Learning Based Multi-modal Addressee Recognition in Visual Scenes with Utterances},
  author    = {Thao Minh Le and Nobuyuki Shimizu and Takashi Miyazaki and Koichi Shinoda},
  booktitle = {Proceedings of the Twenty-Seventh International Joint Conference on
               Artificial Intelligence, {IJCAI-18}},
  publisher = {International Joint Conferences on Artificial Intelligence Organization},             
  pages     = {1546--1553},
  year      = {2018},
  month     = {7},
  doi       = {10.24963/ijcai.2018/214},
  url       = {https://doi.org/10.24963/ijcai.2018/214},
}
```
