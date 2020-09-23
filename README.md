# Depression-Tweets-2019-to-2020
Deep Tweet "Depression"
#Use this to load Twitter json object into python
#https://stackoverflow.com/questions/55929752/how-to-load-twitter-json-object-into-python
#2250 tweets with depression
#2937 twwts without depreesion
dat=list()
with open ('/depression_file.json', 'r') as f:
    for l in f.readlines():
        if not l.strip (): # skip empty lines
            continue

        json_data = json.loads (l)
        dat.append(json_data)
