````markdown
# Instagram Post Upload Simulation (Python)

Hi! 👋

This is a small project where I tried to simulate how uploading a post works on Instagram.  
Obviously, Instagram has a huge backend system, but here I made a simple version in Python.

---

## What it does

- Lets a "user" upload an image with a caption.
- Checks if the image is uploaded and if the caption is there.
- Only allows certain image formats (`.jpg`, `.jpeg`, `.png`).
- Generates unique IDs for posts and images.
- Saves the "image" in a fake storage (just a dictionary in Python).
- Saves the post details in a fake database (a list of posts).

---

## How to use it

1. Open the `Instagram_Post_Upload.ipynb` notebook in Jupyter Notebook.
2. Run **Cell 1** to set up storage and database.
3. Run **Cell 2** to define the upload function.
4. Run **Cell 3** to test uploading a post.
5. Run **Cell 4** to see all the posts in the fake database.

---

## Example

If we run the function like this:

```python
upload_post(
    user_id="prem_001",
    image_file="photo.png",
    caption="Enjoying the view!"
)
````

It will return something like:

```
'Post uploaded successfully! Post ID: <some-unique-id>'
```

And `DATABASE` will have:

```python
[{
  'post_id': '<some-unique-id>',
  'user_id': 'prem_001',
  'image_url': 'storage/<file-id>',
  'caption': 'Enjoying the view!',
  'created_at': '2025-11-15T...'
}]
```

---

 Notes

* This is **just a simulation**. No real images are uploaded anywhere.
* Everything is stored **in memory** using Python lists and dictionaries.
* Purpose is to **understand how backend logic works** for a post upload.





