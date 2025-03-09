import { FaGithub, FaLinkedin, FaXTwitter, FaDev } from "react-icons/fa6";
import { MdEmail } from "react-icons/md";
import { Button } from "@/components/ui/button";

export default function Home() {
  return (
    <div className="min-h-screen flex flex-col items-center justify-center bg-gray-100 text-black p-8">
      <nav className="w-full flex justify-between items-center p-4 max-w-4xl">
        <h1 className="text-2xl font-bold">AJ<span className="text-blue-500">.</span></h1>
        <div className="flex space-x-6">
          <a href="/" className="text-lg" aria-label="Home">HOME</a>
          <a href="/projects" className="text-lg" aria-label="Projects">PROJECTS</a>
          <a href="/blogs" className="text-lg" aria-label="Blogs">BLOGS</a>
          <a href="/about" className="text-lg" aria-label="About">ABOUT</a>
        </div>
      </nav>
      <div className="text-center mt-20">
        <p className="text-gray-500">>_ HI I AM</p>
        <h1 className="text-6xl font-bold mt-2">Aditya</h1>
        <p className="text-xl text-gray-700 mt-2">I am a <span className="text-black font-semibold">ML Researcher</span></p>
        <p className="text-blue-600 font-semibold mt-4">Contributor @ SSoC'24, GSSoC'24 & Hacktoberfest</p>
        <div className="flex justify-center space-x-6 mt-6">
          <a href="mailto:example@gmail.com" aria-label="Email"><MdEmail size={30} /></a>
          <a href="https://github.com" target="_blank" rel="noopener noreferrer" aria-label="GitHub"><FaGithub size={30} /></a>
          <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn"><FaLinkedin size={30} /></a>
          <a href="https://twitter.com" target="_blank" rel="noopener noreferrer" aria-label="Twitter"><FaXTwitter size={30} /></a>
          <a href="https://dev.to" target="_blank" rel="noopener noreferrer" aria-label="Dev.to"><FaDev size={30} /></a>
        </div>
        <div className="mt-6">
          <Button className="bg-blue-600 text-white px-4 py-2 rounded-lg">Resume ⬇</Button>
        </div>
      </div>
    </div>
  );
}
