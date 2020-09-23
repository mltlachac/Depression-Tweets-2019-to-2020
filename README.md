dat=list()
with open ('/Users/Mallak/Desktop/depression_geo.json', 'r') as f:
    for l in f.readlines():
        if not l.strip (): # skip empty lines
            continue

        json_data = json.loads (l)
        dat.append(json_data)
