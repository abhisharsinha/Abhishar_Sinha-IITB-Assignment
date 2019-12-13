PROJECT STRUCTURE


├── attention-ocr    --->    library to train and test ocr model
├── checkpoints    --->    contains model checkpoints at different training steps
├── datasets    --->    contains training and test data
├── exported-model    --->    contains models exported in SavedModel format
├── history   --->   contains loss vs steps data and plot, and model config for every train run
├── static
    ├── index.html    --->    webpage where user can upload images to get json response
├── test_logs    --->    contains predicted vs actual texts for each test run
├── text_renderer    --->    library to generate text images
└── utility_scripts
    ├── create_annotate_data.py    --->    makes annotation file generated by text-renderer suitable for use by attention-ocr
    ├── crop_backgrounds.py    --->    splits an image into 6x6 grid and saves each part
    ├── gen_email_mob.py    --->    generates fake emails and numbers
    ├── get_alphabet.py    --->    gives the alphabet set by traversing through labels
    ├── merge_tfrecords.py    --->    merges multiple tfrecords files into a single file
    ├── only_english.py    --->    removes non-english and non-numeric labels from annotations
    └── testing_inception.ipynb    --->    used to get index of mixed5 layer from layers list of keras inceptionV3 model
├── app.py    --->    flask web app that lets users upload text images and returns json response
├── daily_logs.md    --->    daily log of completed tasks
├── instructions.txt    --->    instructions to run app
├── make_predictions.py   --->   generates predictions in <img_name> <predicted_text> format
├── my_run.sh    --->    runs make_predictions.py
├── requirements.txt    --->    requirements to run the web app
├── train_model.sh    --->    used to train model

