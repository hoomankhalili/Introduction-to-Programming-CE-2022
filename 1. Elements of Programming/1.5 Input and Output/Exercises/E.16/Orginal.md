Given the positions and masses of a sequence of objects, write a program to compute their center-of-mass or centroid. The centroid is the average position of the n objects, weighted by mass. If the positions and masses are given by $(x_i, y_i, m_i)$, then the centroid $(x, y, m)$ is given by:

$$ m  = m_1 + m_2 + ... + m_n $$

$$ x  = (m_1x_1 +  ... + m_nx_n) / m $$

$$ y  = (m_1y_1 +  ... + m_ny_n) / m $$

Write a program Centroid.java that reads in a sequence of positions and masses $(x_i, y_i, m_i)$ from standard input and prints out their center of mass $(x, y, m)$. Hint: model your program after Average.java.
