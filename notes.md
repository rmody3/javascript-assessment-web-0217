Build out the following methods on the CommentsController class (Use ES6 syntax)

CommentsController.prototype.addCommentFormListener()
  iterates through each comment form and adds an eventlistener to trigger a function on form submit
  function should grab the imageId + comment and create a new Comment with those arguments
  execute the render function on that found image object to append the new comment

CommentsController.prototype.render(commentObject)
  selects the appropriate ul for this comment to be added to
  appends the new comment element to this ul
  Don't try to copy the ImagesController.render function because that is implemented differently

Build the following on the comment class model (Use ES6 syntax)

new Comment(comment, imageId)
  should initialize with an id, image object (findImage) and commentContent (the actual text of the comment)
  should save new comment to Comment.all property

Comment.all
  should return all of the comment objects in an array
  a property of the Comment class

Comment.prototype.findImage(imageId)
  given an int for an image id, returns the image object with that id
  before return - adds current comment to image's comments property

Comment.prototype.commentEl()
  returns a string of html
  html has an li tag with an id field and shows the comment
