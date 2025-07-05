
## 📦 Model Conversion

To convert an HDF5 model to TensorFlow\.js format, use the `tensorflowjs_converter` CLI tool:

```bash
tensorflowjs_converter --input_format keras --output_format tfjs_graph_model model/keypoint_classifier/keypoint_classifier.hdf5 tfjs_model/
```

Refer to the [TensorFlow.js conversion guide](https://www.tensorflow.org/js/guide/conversion) for more details.

---

##  Getting Started

To run the development server:

```bash
yarn dev
```

Once started, open your browser at:

```
http://localhost:3000
```

---

## ⚠ Notes

* This project was originally built using **Next.js**. Due to issues with Server-Side Rendering (SSR), it was migrated to **Vite** for a simpler and static setup.
* The GitHub Pages CI pipeline may not work out-of-the-box. Ensure that your **deployment folder is correctly configured** in the GitHub Actions workflow (`dist` for Vite).
* If gesture recognition models fail to load, make sure the correct **public path** or **environment variables** are set (especially `NEXT_PUBLIC_BASE_PATH` or similar) to locate model files under the `public/` directory.



