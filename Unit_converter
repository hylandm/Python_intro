print "Welcome Michael Hyland\'s Unit Converter! :)"
print "You can convert Distances, Weights, Volumes & Times to one another, but only"
print "within units of the same category, which are shown below. E.g.: 1 mi in ft"
print
print "Distances: ft cm mm mi m yd km in"
print "Weights: lb mg kg oz"
print "Volumes: floz qt cup mL L gal pint"

distances = {'ft':3.28084,'cm':100,'m':1,'mm':1000,'mi':.000321371,'yd':1.09361,'km':.001,'in':39.3701}
weights = {'lb':2.20462,'mg':1000000,'kg':1,'oz':35.274}
volumes = {'L':1,'floz':33.814,'qt':1.05669,'cup':4.22675,'mL':1000,'gal':.264172,'pint':2.11338}

while 1:
    ipt = raw_input("Convert [AMT SOURCE_UNIT in DEST_UNIT, (q)uit, (h)elp, or (u)nits]:")
    if ipt == 'q' or ipt == 'quit':
        break
    if ipt == 'h' or ipt == 'help':
      print 'Type in the following format [<number> "unit which number represents" in "unit to convert to"]'
      continue
    if ipt =='u' or ipt == 'units':
        print 'Acceptable units are...'
        print "Distances: ft cm mm mi m yd km in"
        print "Weights: lb mg kg oz"
        print "Volumes: floz qt cup mL L gal pint"
        continue
    iptarr = str.split(ipt) #split the input into strings based on whitespace
    if len(iptarr) != 4:
        print "Incorrect format. Please enter in the format shown below"
        continue
    amount = float(iptarr[0])
    srcunit = iptarr[1]
    destunit = iptarr[3]
    if distances.has_key(srcunit):
        if not distances.has_key(destunit):
            print 'Your destination unit is not recognized! type "units" to see list of available units'
            continue
        print (amount/distances[srcunit])*distances[destunit]
    elif weights.has_key(srcunit):
        if not weights.has_key(destunit):
            print 'Your destination unit is not recognized! type "units" to see list of available units'
            continue
        print (amount/weights[srcunit])*weights[destunit]
    elif volumes.has_key(srcunit):
        if not volumes.has_key(destunit):
            print 'Your destination unit is not recognized! type "units" to see list of available units'
            continue
        print (amount/volumes[srcunit])*volumes[destunit]
    else:
        print 'Source unit not recognized! Please ensure your format is correct and that your unit is listed below.'
        print
        print "Distances: ft cm mm mi m yd km in"
        print "Weights: lb mg kg oz"
        print "Volumes: floz qt cup mL L gal pint"
