1) The file ```preprocessing_dataset.py``` is used for preprocessing the dataset (.json) file.
2) For balancing the dataset, pass arguements ```mode = 'balanced'``` and ```task = {required_task}``` to the ```preprocess_data``` method.
3) The common backbone method is implementend in files starting with ```common...``` and the individual backbone per task is implemented on ```individual...``` files.
4) The specific loss function and settings are mentioned in the file name. For example, the file named ```individual_bert_exact_all_losses_mistake_identification``` consists of bert model in exact setting for all losses.
5) The ```common..``` file consists everything in a single file.
6) Each notebook can be ran independtly.
