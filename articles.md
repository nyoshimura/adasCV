<table width="100%">
  <tr>
    <td></td>
    <td colspan=2 align=center>Summary</td>
  </tr>
  <tr>
    <td align=center>**Blog**</td>
    <td align=center>English</td>
    <td align=center>Tweet</td>
  </tr>

  <tr>
    <td width="25%">[Lane Detection with Deep Learning (Part 1)](https://towardsdatascience.com/lane-detection-with-deep-learning-part-1-9e096f3320b7)
    ![](https://cdn-images-1.medium.com/max/1600/1*zx73GA3OTXtXietEMNDXDQ.png)
    </td>

    <td align=center width="35%">Blog post on **towardsdatascience.com**.
    Traditional approach for lane detection is highly depending on camera spec or mounting position, available in limited situations, and quite slow (4.5fps).
    To build deep neural network, driving data was collected by smart-phone and labeling was done by old-CV algorithms + manually correction.
    Label is six polynomial coefficients (a,b, c in <img src="http://www.sciweavers.org/tex2img.php?eq=a%7Bx%7D%5E2%2Bbx%2Bc&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="a{x}^2+bx+c" width="107" height="19" /> of left/right lane).
    To increase data at curve, rotation is applied for augmentation.
    </td>
    <td>
    <blockquote class="twitter-tweet" data-lang="en"><p lang="ja" dir="ltr">従来のレーン認識はカメラのFOV, 取り付け位置などHWへの依存が強く、カーブや道路の傷で誤認識しやすく、処理が重い。ので、CNN使おうと考えたけどデータセット作り意外と大変だったぜというおはなし。2へ続く。<br><br>“Lane Detection with Deep Learning (Part 1)” by <a href="https://twitter.com/MVirgs44?ref_src=twsrc%5Etfw">@MVirgs44</a> <a href="https://t.co/f3yFA4mR8n">https://t.co/f3yFA4mR8n</a></p>&mdash; ysmrnbt (@ysmrnbt) <a href="https://twitter.com/ysmrnbt/status/1021197056893902848?ref_src=twsrc%5Etfw">July 23, 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></td>
  </tr>
  <tr>

  <td width="25%">[Lane Detection with Deep Learning (Part 2)](https://towardsdatascience.com/lane-detection-with-deep-learning-part-2-3ba559b5c5af)
  <br><br>
  ![](https://cdn-images-1.medium.com/max/1000/1*0Eg4sdSjVJCaZzFNdwJ9JA.png)
  </td>

  <td align=center width="35%">Blog post on **towardsdatascience.com**.
  Predicting polynomial coefficients is not so robust using CNN + Fully Connected layers, so switched to use semantic segmentation approach. Training dataset is 12764 images incl. augmented(rotated or flipped) images, input size is 80x160x3, and SegNet-based architecture is used. Inference speed is 25fps w/ GPU (5.5fps w/o GPU) and detection result is improved, but left/right boundaries are not consistent yet.
  </td>
  <td>
  <blockquote class="twitter-tweet" data-lang="en"><p lang="ja" dir="ltr">CNN+FCで曲率推定だとレーンをちゃんと見てくれないのでSegNetベースで実装。処理も25fpsと速く安定性も増した(?)が暗闇や道路の傷にはまだ反応してる様子。<br><br>“Lane Detection with Deep Learning (Part 2)” by <a href="https://twitter.com/MVirgs44?ref_src=twsrc%5Etfw">@MVirgs44</a> <a href="https://t.co/fLdLMyYA7R">https://t.co/fLdLMyYA7R</a></p>&mdash; ysmrnbt (@ysmrnbt) <a href="https://twitter.com/ysmrnbt/status/1021221409425539073?ref_src=twsrc%5Etfw">July 23, 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</td>
  </tr>
  <tr>
    <td>**Paper**</td>
    <td align=center>English</td>
    <td align=center>Tweet</td>
  </tr>
  <tr>
    <td>Deep Learning Lane Marker Segmentation From Automatically Generated Labels</td>
    <td align=center>WIP</td>
    <td align=center>WIP</td>
  </tr>
</table>
