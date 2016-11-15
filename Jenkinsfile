node ('VerifyAnims') {
    def workspace = pwd()
    def text = readfile "${workspace}/Windshield.caproj"
    def match = text =~ /<object-type name="(.+)" sid=".+">\n            <plugin id="Sprite" \/>/
    def fileName = match[0][1]
    if (fileExists ("${workspace}/Animation/"+fileName+"/Default/000.png")) {
           echo "Yes it does exist!"
    }
}