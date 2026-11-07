# Blender Colab Renderer

Render Blender animations using Cycles in Google Colab. The notebook supports saving frames to Google Drive and resuming interrupted renders. EEVEE is not supported.

[Open in Colab](https://colab.research.google.com/github/Deanx270/blender-colab-renderer/blob/main/Blender_Cloud_Renderer.ipynb)

## Usage

1. Open the notebook in Colab and select a GPU runtime.
2. Upload your `.blend` file to `/content` or place it in `MyDrive/BlenderRender` if using Google Drive. Make required external assets available alongside the project.
3. Run the installation cell, configure the render settings, and run the controller cell.
4. Find the MP4 in Google Drive or `/content`, depending on your storage setting.

The notebook downloads a Blender daily build and overrides scene settings, including the render engine, samples, bounce limits, compositing, motion blur, and denoising. These changes can affect the result. When resume is disabled, existing frames in the selected output frame folder are deleted before rendering.

## License

[MIT](LICENSE)
