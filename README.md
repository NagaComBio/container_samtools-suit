# singularity_samtools-suit
Singularity image for samtools suit (samtools, htslib, bcftools)

# To build
sudo docker build --build-arg SUIT_VERSION=1.9 -f build_samtools_perlenv.def -t ghcr.io/nagacombio/container_samtools-suit:v1.9 .

# To push
echo $CR_PAT | docker login ghcr.io -u NagaComBio --password-stdin
sudo docker push ghcr.io/nagacombio/container_samtools-suit:v1.9
