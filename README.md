# search-a-keyword-into-a-txt-file
python script that search for a specific word in a txt file and cleans the list from chosen keywords. extracted in a txt file
with open("input_file.txt") as openfile:
for line in openfile:
 for part in line.split():
  if "ship" in part:
   f= open ("output_file.txt","a")
    print ( line , file=f)
    f.close()
    delete_list = ["airship", "friendship" ]
    with open("output_file.txt", "r") as fin, open("cleaned_file.txt", "w+") as fout
    for line in fin:
      for word in delete_list:
       line = line.replace(word, "")
        fout.write(line)

