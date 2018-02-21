# Comments in DIYbiosphere
This repository is used to display comments in the webpages of DIYbiosphere

## How to open an Issue
Open an Issue with the `title: ` of the webpage. In the description, add a link back to the webpage

## How to enable comments on a webpage
After you created the issue:
- Go to `_data/entry_issue.yml` file in the [diybiosphere/sphere](https://github.com/DIYbiosphere/sphere) repository
- Add the following code:
```yml
- doc_name: diybiosphere # file_name, NOT title. Same as URL.
  comments_issue: 2 # issue number for comments in diybiosphere/comments
  edit_issue: 1 # issue number for discussing editing in diybiosphere/sphere
```
- Commit and wait for the build to go through Travis. It might take a few minutes

### doc_name
the `doc_name:` is NOT the title, it is the _file name_ in the repository. 

If you are not sure of the file name, just look at  the URL. The last word after the last slash should be the file name. `i.e. http://sphere.diybio.org/labs/AvocadoLab`, file name is `avocadolab`

### edit_issue
Issues in _this_ repository are meant to show in the webpages and _discuss the content_ in the webpage. 

To discuss errors or problems or any issue in terms of _editing the content_ in the entry, an issue should be opened in the [diybiosphere/sphere](https://github.com/DIYbiosphere/sphere) repository. NOT HERE.
