# Zenika Training: Introduction to Web Accessibility

This repo contain all the training material for the **Introduction to Web Accessibility** training.


## Run the training

Regardless of the method used to run the training, PDF are outputted in the `pdf` folder. While served, slides are accessible at https://localhost:8080/slides.html and exercices are accessible at https://localhost:8080/labs.html


### With NPM

```bash
# Intall local dependencies
npm install

# Serve slides and exercices localy
npm start

# Output slides and exercices as PDF
npm run pdf
```


### With Docker

```bash
# Serve slides and exercices localy
docker run -it --rm -p 8080:8080 -v $(pwd):/training-material zenika/sensei

# Output slides and exercices as PDF
docker run -it --rm -p 8080:8080 -v $(pwd):/training-material --cap-add SYS_ADMIN zenika/sensei pdf
```


## Update the training material

Pull request to improve that material is more than welcome.

This repos use [@zenika/sensei](https://github.com/Zenika/sensei) to drive the training, see [its documentation for details](https://github.com/Zenika/sensei/blob/master/README.md).

All slides are markdown files within the `Slides` folder, feel free to add new ones or to update existing ones. Exercices are markdown files within the `CahierExercices` folder.
