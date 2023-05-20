# Feature Extraction
the note book provide multiple functions

## check_timestamps(path)
    iterates over each csv in the given directory, and check the homogenity of "timestamps" column
    prints out every sampling period that was observed in each dataframe
    
    attributes    
        path : the path of the data (csv) directory

    return: None

## interpolate_dataset(path, dt)
    interpolate every channel of every dataframe at the given directory to create homogenous sampling
    the function stores the interpolated signals at a directory called "interpolated_signals" created at the same relative path of the script if the directory exist then the files will be overwritten

     attributes    
        path : the path of the data (csv) directory
        dt   : sampling period
    return: None

## create_eeg_features_empty_dataset(path)
    creates an instance of the dataset header with the header of the dataframe
    
    attributes

        path : the path of the data (csv) directory
        
    return: an empty pandas dataframe, wih only the headers

## extract_features(dataset,path)
    creates an instance of the dataframe header with the header of the dataframe
    
    attributes
        dataset : a dataframe initialized by the function create_eeg_features_empty_dataset(path)
        path    : the path of the data (csv) directory

    return: the dataset with all the features and records 

## export_to_csv(dataset)
    save the dataframe as csv file with name "dataset.csv" for later uses
    
    attributes
        dataset : a dataframe initialized by the function create_eeg_features_empty_dataset(path)
    return: None

## power_spectral_density_features(signal, fs=1/0.004)
    calculate the features related to the power spectral density

    attributes
        signal : numpy array of the signal
        fs : sampling frequency
    return: entropy , sef (Spectral edge frequency), peak_freq (Spectral peak frequency)

## calculate_plv(signal1, signal2, fs)
    calculate the Phase synchronization which is a measure of the synchronization of the phase angles of two EEG signals at different electrode sites

    attributes
        signal1 : numpy array of the first signal
        signal2 : numpy array of the second signal
        fs : sampling frequency

    return: array of size 5, the synchronization of each brain wave frequency band {𝛼, β, 𝜃, 𝛿, 𝛾}


# To use the provided functions 
    if its only for exploration it would be recommended to run "feature extraction.ipynb" cell by cell 

    or to use the provided functions as follows

    '''
        if __name__ == "main":
            check_timestamps(path)
            interpolate_dataset(path, dt)
            dataset = create_eeg_features_empty_dataset(path)
            dataset = extract_features(dataset,path)
            export_to_csv(dataset)
    '''