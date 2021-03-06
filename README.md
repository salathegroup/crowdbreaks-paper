# Crowdbreaks: Tracking Health Trends using Public Social Media Data and Crowdsourcing
This repository contains all additional code/data/analysis for the paper "Crowdbreaks: Tracking Health Trends using Public Social Media Data and Crowdsourcing".

If you use the data or model please cite the work like this
```
Müller, Martin M., and Marcel Salathé. "Crowdbreaks: Tracking health trends using public social media data and crowdsourcing." Frontiers in public health 7 (2019).
```
or
```bibtex
@article{muller2019crowdbreaks,
  title={Crowdbreaks: Tracking health trends using public social media data and crowdsourcing},
  author={M{\"u}ller, Martin M and Salath{\'e}, Marcel},
  journal={Frontiers in public health},
  volume={7},
  year={2019},
  publisher={Frontiers Media SA}
}
```

## Install
```
conda env create -f environment.yml
```

## Download tweets
Generate a set of Twitter API keys and download the tweets using the following command:
```
python download_tweets.py -i ./data/vaccine_sentiment_data.csv -o ./data/tweets.jsonl --consumerkey XXX --consumersecret XXX --accesstoken XXX  --accesssecret XXX
```

## Download vaccine sentiment model
```
wget https://crowdbreaks-public.s3.eu-central-1.amazonaws.com/models/fasttext_v1.ftz -o ./data/fasttext_v1.ftz
```
