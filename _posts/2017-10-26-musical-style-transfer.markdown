---
layout: default
title:  "'Style' Transfer for Musical Audio Using Multiple Time-Frequency Representations"
date:   2017-05-20 01:22:52 -0400
categories: jekyll update
author:
- anonymous
---
This blog post is a supplement to the paper, "'Style' Transfer for Musical Audio Using Multiple Time-Frequency Representations". 
<!--4. A naive (no prior training for source audio) method for source separation using this framework.-->

# Experiment 4.1: Musical Texture Generation

<body>
	<center> Figure 4: Columns 1 and 3: comparison of inter-onset lengths distribution and KL divergence from the source distribution for a texture generation example as the effective receptive field increases in time. Columns 2 and 4: mean local autocorrelation plots showing the increase in hierarchical rhythmic structure of the audio without any significant increase in the maximum cross-correlation value.
	<img src="/rhythmic_structure_plots.PNG" width="20">
</center>
</body>	

<center>

<table>

	<!-- Crazy -->
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 1</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Source</th>
		<td>
			<iframe width="560" height="315" src="https://www.youtube.com/embed/Qe500eIK1oA" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Textures</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="300" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363221006&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true&amp;visual=true"></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 2</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Source</th>
		<td>
			<iframe width="560" height="315" src="https://www.youtube.com/embed/idGvKFbYgI4?start=255&&end=315" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Textures</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="300" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363220177&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true&amp;visual=true"></iframe>
		</td>
	</tr>
</table>

</center>

# Experiment 4.2: Testing Key Invariance

<body>
	<center> Figure 5: Comparison of the error with different content-based representations for a task where the content and style audio is exactly the same except for key. The x-axis represents varying semi-tone offsets in musical representation. The first point on the left of 0 semi-tone offset represents a trivial problem where both content and style are exactly the same signals. We plot the error in the log-magnitude STFT representations to show the overall signal error.
	<img src="/updated_content_plot.png">
</center>
</body>	

<center>

<table>

	<!-- Crazy -->
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Source</th>
		<td style="text-align: center; vertical-align: middle;">
		<iframe width="100%" height="166" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/348891202&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">STFT Reconstructions</th>
		<td style="text-align: center; vertical-align: middle;">
		<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363224677&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Mel Reconstructions</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363224301&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">CQT Reconstructions</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363224449&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Mel + CQT Reconstructions</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363224575&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>

</table>

</center>

# Experiment 4.3: Comparison of examples with best implementation.

<center>

<table>

	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 1</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/fJ9rUzIMcZQ?start=220&&end=290" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/WSeNSzJ2-Jw?start=0&&end=116" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Results</th>
		<td style="text-align: center; vertical-align: middle;">
		<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363228481&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>

	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 2</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/Fe93CLbHjxQ?start=11&&end=62" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/4D7u5KF7SP8?start=0&&end=240" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Results</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363230506&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>

		<!--     Jacob Collier -->
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 3</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/EkPy18xW1j8?start=15&&end=45" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/cttFanV0o7c?start=5&&end=74" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Result</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="166" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/348897860&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>
		<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 4</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/cvChjHcABPA?start=38&&end=68" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/UxxajLWwzqY?start=35&&end=95" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Result</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363233983&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>	
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 5</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/_MBRFbHHNzg?start=0&&end=30" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/FTQbiNvZqaY?start=4" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Result</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/363933307&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>	
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 6</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/9SOryJvTAGs?start=90&&end=120" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/5abamRO41fE?start=64&&end=94" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Result (Content - Mel+CQT, Style - Mel (2 Resid) + CQT (3 resid)</th>
		<td style="text-align: center; vertical-align: middle;">
			<audio controls>
      <source src="/loveshack_melcqt.wav">
      </audio>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Result (Content - STFT, Style - Mel (2 Resid) + CQT (3 resid)</th>
		<td style="text-align: center; vertical-align: middle;">
			<audio controls>
      <source src="/loveshack_stft.wav">
      </audio>
		</td>
	</tr>	
	<tr>
		<th style="text-align: center; vertical-align: middle;"></th>
		<th style="text-align: center; vertical-align: middle;">Example 7</th>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Content</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/hNv5sPu0C1E?start=10&&end=20" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Style</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/w5x_9KEogM8?start=0&&end=20" frameborder="0" allowfullscreen></iframe>
		</td>
	</tr>
	<tr>
		<th style="text-align: center; vertical-align: middle;">Result</th>
		<td style="text-align: center; vertical-align: middle;">
			<iframe width="100%" height="166" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/349294441&amp;color=%23ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;show_teaser=true"></iframe>
		</td>
	</tr>		
