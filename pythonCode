if hou.selectedNodes()==() :
    print("please select")
    hou.ui.displayMessage("Bhai node toh select kar")
#print(hou.selectedNodes())
if hou.selectedNodes()!=() :
    aNode = hou.selectedNodes()[-1]
    
    bnc = aNode.createOutputNode('attribwrangle','boneNumberChecker_{0}_01'.format(aNode.name()))
    #bnc.moveToGoodPosition()
    #bnc.setCurrent(True, clear_all_selected=True)
    bnc.setParms({"snippet":"s[]@myTransformNames= agenttransformnames(0, @primnum);\nif(@ptnum==0)\n{\nforeach(int num;string item;@myTransformNames)\n{\nprintf('bone number %d is %s\\n',num, item);\n}\n}\nvector a;"})
    
