# Efficient Tensor Product exp for Efficiency (Preview)

Tianlang

### Preview before Releasing

- Results include:

    - Comparison with e3nn (Equivariant Feature Interaction)
        - Results shown `test_equi_feat.ipynb`
        - Upper Left of Fig 1
    
    - Comparison with eSCN (Equivariant Convolution)
        - Results shown `test_equi_conv.ipynb`
        - Upper Middle of Fig 1

    - Comparison with MACE (Equivariant Many-Body Interaction)
        - Results shown `test_equi_many-body.ipynb`
        - Upper Right, Down Left and Down Middle of Fig 1


- Main Revision
    - Make code more accessible
        - More comments added
        - Rename some of the variable to help beter understanding
    - Adjust the code for fairer comparison 
        - e.g., As previously discussed, the e3nn TP is redefined (retraced) in every loop. Now the code is slightly adjusted so that TP is defined once and reused, which makes comparsion fairer and closer to real application in NNs.