# thegitopsfridge

## step zero A: essentials and everything on the list is covered, no more candy than intended, single point of truth what is actually there
oc apply -f 00a-fillthefridgeright-application.yaml

## step zero B: if not I forgot it, but my spouse initially - now thats easy.
oc apply -f 00b-fillthefridgeright-application.yaml
## step one: isolate
oc apply -f 01-therottenoranges-application.yaml

## step two: how about the little thieves
### two A - delete deployment
--> pretend "I" am such a thief, take smth out and I am veryyy hungry
oc delete deployment milkcarton -n topofthefridge
### two B - add an idp
--> I probably couldnt image how they much would eat if the fridge really worked that way... it solves my, but causes new probs, I need something else
--> lets put a lock:
oc apply -f fingerweg-application.yaml

## three
### three a - put things out of the cluster
oc apply -f 03a-getstuffout-application.yaml

### three b - lets just increase it size
oc apply -f 03b-enlargeit-application.yaml

outlook:
next time I'll bring some more fridges ... and you probably know what happens then :)


