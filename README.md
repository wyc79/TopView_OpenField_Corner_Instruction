#  Labeling of Corners



1. add video to the project using `Add new videos`

<video src="./readme_resources/add_video.mp4" type="video/mp4" controls>Demo video: add video. Your browser does not support the video tag.</video>



2. Once added to project, extract frame 

<video src="./readme_resources/extract_frame.mp4" type="video/mp4" controls>Demo video: extract frame. Your browser does not support the video tag.</video>

Check the extracted frames in the `labeled-data` folder, 3 images should be created. Only one frame for each video is needed for this task, I set extraction to 3 just in case there are any blurry/blocked corners. 

<video src="./readme_resources/check_folder.mp4" type="video/mp4" controls>Demo video: check extracted frames. Your browser does not support the video tag.</video>




3. Label the frames. Default order is: TopLeft - TopRight - BottomLeft - BottomRight. Always check if you are labeling the right corner (by checking the color and `keypoint` tab on the lower right corner of the window). Use another frame if the one or more corners are blocked by the animal.

<video src="./readme_resources/label_frame.mp4" type="video/mp4" controls>Demo video: label frame. Your browser does not support the video tag.</video>



4. Transfer the results into the Excel sheet. Remember to check the ordering of coordinates.

<video src="./readme_resources/save_result.mp4" type="video/mp4" controls>Demo video: save result. Your browser does not support the video tag.</video>

Additional validation: most corner coordinates should be relatively the same, especially if collected on the same date. Remember to double-check the frames and labeling if the differences within the same day are large.





5. Fill out the `Labeled?` and `Relative Path` column

   `Labeled?`: change to `Y` after coordinated pasted

   `Relative Path`: Relative path of the video to the folder, for example, the relative path of video `wt817_day11_2024-05-13_16-51-34` will be `./videos/20240513/wt817_day11_2024-05-13_16-51-34.mp4` (For windows users: change `\` to `/` in path)



Here is an example of the end result:

| Filename                        | TopLeft_x   | TopLeft_y  | TopRight_x  | TopRight_y  | BottomLeft_x | BottomLeft_y | BottomRight_x | BottomRight_y | Primary Labeled By: | Labeled? | Checked by: | Checked? | Relative Path                                         |
| ------------------------------- | ----------- | ---------- | ----------- | ----------- | ------------ | ------------ | ------------- | ------------- | ------------------- | -------- | ----------- | -------- | ----------------------------------------------------- |
| ...                             |             |            |             |             |              |              |               |               |                     |          |             |          |                                                       |
| wt817_day11_2024-05-13_16-51-34 | 129.0631245 | 66.6757796 | 481.3163102 | 60.07103237 | 140.0710366  | 413.4250092  | 479.1147278   | 402.4170972   | Yuanchen            | Y        |             |          | ./videos/20240513/wt817_day11_2024-05-13_16-51-34.mp4 |
| ...                             |             |            |             |             |              |              |               |               |                     |          |             |          |                                                       |
