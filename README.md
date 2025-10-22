# Pore-scale-Reactive-Flow
A public dataset of pore-sacle reactive flow process
The fluid flow coupled with reactive transport with first-order chemical reaction on solid surafce inside porous media is the typical problem in energy-related and chemical engineering. This dataset provides 2000 sets of reactive flow data generated from finite element simulation in COMSOL.
The dataset is in form of point cloud, where points are extracted from vertices in finite element mesh. Besides, the dataset performs point-sampling on the complex porous domain, including farthest point class, curvature distributed class, boundary class and solid geometry class.

The dataset is structured as follows:

Fluid flow:{
    "inlet": inlet_tensor_f, "inlet_mask": inlet_mask_f,
    "outlet": outlet_tensor_f, "outlet_mask": outlet_mask_f,
    "side": side_tensor_f, "side_mask": side_mask_f,
    "solid": solid_tensor_f, "solid_mask": solid_mask_f,
    "uniform": uniform_tensor_f, "uniform_mask": uniform_mask_f,
    "curvature": curvature_tensor_f, "curvature_mask": curvature_mask_f,
}

Concentration transport:{
    "inlet": inlet_tensor_r, "inlet_mask": inlet_mask_r,
    "outlet": outlet_tensor_r, "outlet_mask": outlet_mask_r,
    "side": side_tensor_r, "side_mask": side_mask_r,
    "solid": solid_tensor_r, "solid_mask": solid_mask_r,
    "uniform": uniform_tensor_r, "uniform_mask": uniform_mask_r,
    "curvature": curvature_tensor_r, "curvature_mask": curvature_mask_r,
}

The visualization of point sampling is:
<img width="712" height="568" alt="image" src="https://github.com/user-attachments/assets/d1d1c7de-a75d-4360-ad3b-133445deeb36" />

