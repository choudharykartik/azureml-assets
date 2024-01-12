# Description
This is a 7B parameter, based on Llama2, trained on Hindi, English, and Hinglish. 
More details about the model, its training procedure, and evaluations can be found [here](https://www.sarvam.ai/blog/announcing-openhathi-series).



#### License
OpenHathi-7B-Hi-v0-1-Base is made available under the lamma2 license.

# Inference samples

Inference type|Python sample (Notebook)|CLI with YAML
|--|--|--|
Real time|<a href="https://aka.ms/azureml-infer-online-sdk-text-generation-dolly" target="_blank">text-generation-online-endpoint.ipynb</a>|<a href="https://aka.ms/azureml-infer-online-cli-text-generation-dolly" target="_blank">text-generation-online-endpoint.sh</a>
Batch |<a href="https://aka.ms/azureml-infer-batch-sdk-text-generation" target="_blank">text-generation-batch-endpoint.ipynb</a>| coming soon

## Sample input (for real-time inference)

```json
{
    "input_data": {
        "input_string": [
            "What is meaning of life?"
        ],
        "parameters": {
            "temperature": 0.5,
            "top_p": 0.5,
            "max_new_tokens": 200,
            "do_sample": true
        }
    }
}
```

## Sample output
```json
[
    {
        "0": "What is meaning of life?\n---\nजीवन का अर्थ एक जटिल और बहुआयामी अवधारणा है जो व्यक्तिगत मान्यताओं, मूल्यों और अनुभवों के आधार पर व्यापक रूप से भिन्न होती है। While there is no single answer to this question, many people find meaning in their relationships, their work, their passions, their spirituality, or their contributions to society.\n\nजीवन का अर्थ खोजने के लिए एक व्यक्ति से दूसरे व्यक्ति में बहुत भिन्नता है। Some people find meaning in their family and relationships, while others find meaning in their work or career. कुछ लोग अपने जुनून या रुचियों के माध्यम से अर्थ पाते हैं, जबकि अन्य लोग अपने आध्यात्मिक या धार्मिक विश्वासों के माध्यम से अर्थ पाते हैं।\n\nUltimately, the meaning of life is subjective and can be influenced by a variety of factors, including one's personal experiences, cultural background, and values. जबकि जीवन का कोई एकल अर्थ नहीं है, कई लोग अपने जीवन में अर्थ और उद्देश्य की भावना खोजने के लिए काम करते हैं, जो"
    }
]
```
