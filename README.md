# Django Image Uploader

Django Image Uploader is a simple web application built with Django that allows users to upload and manage images. It provides a user-friendly interface for uploading images, and the uploaded images are stored in the server's file system.

## Features

- **Image Upload:** Users can upload images through a user-friendly interface.
- **Image Management:** Users can view their uploaded images.
- **Responsive Design:** The application is designed to work seamlessly on various devices.

## Prerequisites

Make sure you have the following installed before running the application:

- Python 3.x
- Django (latest version)

## Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/Prasad981998/ImageUploader.git
    ```

2. Install dependencies:to use image field in your project.

    ```bash
    pip install pillow
    ```

3. register media file in setting.py file (at the end).

    ```bash
    MEDIA_URL = '/media/'
    MEDIA_ROOT=BASE_DIR/'media'
    ```

4. modules to import and update urls.py file:

    ```bash
    from django.conf import settings 
    from django.conf.urls.static import static #to show images from myimage

    urlpatterns = [
        
    ] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
    ```

5. Run the development server:

    ```bash
    python manage.py runserver
    ```

6. Open your browser and go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/) to access the application.

## Usage

- Create a new account or log in if you already have one.
- Navigate to the "Upload" section to upload your images.
- Visit the "My Images" section to manage your uploaded images.
- Have fun exploring the features of the Django Image Uploader!

## Contributing

If you'd like to contribute to this project, please follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to the Django community for their amazing framework.

## NOTE
- This project is in development phase many functionalities are in process to update.
