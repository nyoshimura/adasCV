## Summary of blogs / papers

<table width="100%">
  <tr>
    <td></td>
    <td colspan=2 align=center>Summary</td>
  </tr>

  <tr>
    <td align=center><b>Blog</td>
    <td colspan=2 align=center></td>
  </tr>

  <tr>
    <td width="30%" align=center><a href="https://towardsdatascience.com/lane-detection-with-deep-learning-part-1-9e096f3320b7">Lane Detection with Deep Learning (Part 1)
    <br>
    <img src="https://cdn-images-1.medium.com/max/1600/1*zx73GA3OTXtXietEMNDXDQ.png" align="center" border="0" width="300" />
    </td>
    <td colspan=2 align=center>Blog post on <b>towardsdatascience.com</b>.
    Traditional approach for lane detection is highly depending on camera spec or mounting position, available in limited situations, and quite slow (4.5fps).
    To build deep neural network, driving data was collected by smart-phone and labeling was done by old-CV algorithms + manually correction.
    Label is six polynomial coefficients (a,b, c in <img src="http://www.sciweavers.org/tex2img.php?eq=a%7Bx%7D%5E2%2Bbx%2Bc&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="a{x}^2+bx+c" width="107" height="19" /> of left/right lane).
    To increase data at curve, rotation is applied for augmentation.
    <br>
    (<a href="https://twitter.com/ysmrnbt/status/1021197056893902848">Tweet</a>)
    </td>  
  </tr>
  <tr>
  <td width="30%" align=center><a href="https://towardsdatascience.com/lane-detection-with-deep-learning-part-2-3ba559b5c5af">Lane Detection with Deep Learning (Part 2)
  <br><br>
  <img src="https://cdn-images-1.medium.com/max/1000/1*0Eg4sdSjVJCaZzFNdwJ9JA.png" align="center" border="0" width="300" />
  ![]()
  </td>

  <td colspan=2 align=center>Blog post on <b>towardsdatascience.com</b>.
  Predicting polynomial coefficients is not so robust using CNN + Fully Connected layers, so switched to use semantic segmentation approach. Training dataset is 12764 images incl. augmented(rotated or flipped) images, input size is 80x160x3, and SegNet-based architecture is used. Inference speed is 25fps w/ GPU (5.5fps w/o GPU) and detection result is improved, but left/right boundaries are not consistent yet.
  <br>
  (<a href="https://twitter.com/ysmrnbt/status/1021221409425539073?ref_src=twsrc%5Etfw">Tweet</a>)
  </td>
  </tr>
  <tr>
    <td width="30%" align=center><b>Paper</td>
    <td align=center></td>
  </tr>
  <tr>
    <td width="30%" align=center>Deep Learning Lane Marker Segmentation From Automatically Generated Labels</td>
    <td align=center>WIP</td>
  </tr>
</table>
