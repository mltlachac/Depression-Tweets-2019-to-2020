
dat=list()
with open ('/depression_file.json', 'r') as f:
    for l in f.readlines():
        if not l.strip (): # skip empty lines
            continue

        json_data = json.loads (l)
        dat.append(json_data)
