# tamrin1-3....nemodar-shekl
plot(x,
     xlab="Latitude",
     ylab="Longitude",
     pch=3,
     col=result$clust)

points(result$centers,
       pch=19,
       cex=2)

for(i in 1:nrow(x)){

  segments(
    x[i,1],
    x[i,2],
    result$centers[result$clust[i],1],
    result$centers[result$clust[i],2]
  )

}
